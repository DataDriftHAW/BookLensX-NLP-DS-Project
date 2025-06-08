# Use Python 3.10 slim image
FROM python:3.10-slim

# Set working directory in the container
WORKDIR /assignment1

# Avoid interactive prompts during installs
ENV DEBIAN_FRONTEND=noninteractive

# Install system dependencies (for building some Python packages)
RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    git \
    && rm -rf /var/lib/apt/lists/*

# Upgrade pip and install Python dependencies
COPY requirements.txt .
RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

# Download small English model for spaCy
RUN python -m spacy download en_core_web_sm

# Copy your local code into the container
COPY . .

# Optional: Expose port for Jupyter (if needed)
EXPOSE 8888

# Default command: open bash shell (you can customize later)
CMD ["bash"]

