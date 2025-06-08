## The setup process using docker will be added here as we work further

### 1. Install docker from official source: 
        https://www.docker.com/

### 2. Clone the repository to your local drive.


### 3. Go inside the folder 'assignment1' , make sure your vscode terminal is inside the folder

```powershell
cd ./ProjectFolder 
```

### 4. Build the Docker Image:
```powershell
docker-compose build
```
It takes some time to build and install dependencies and linux kernel, so have some patience.


### 5. Run the container:
```powershell
docker-compose up
```
### 6. To access the container terminal or to execute any command inside the terminal
```powershell
docker exec -it nlp_ds_project bash
```
### or if you don't have bash installed inside the container then use sh.
```powershell
docker exec -it nlp_ds_project sh
```

### After building make sure to do this with kernel:
```yml
Kernel : Change Kernel : Select Kernel : Select "Python 3.*" : Always start the preferred kernel : Select 
```

### Anytime building a new docker container, keep in mind that:
```yml
        nlp_ds_project:
        build:
        context: .
        dockerfile: Dockerfile
        container_name: nlp_ds_project
```
