# Assignment 5: Query STAC API for Satellite Imagery

## Instructions

1. **Pull the Docker Image:**

## Prerequisites

- Install Docker: [Get Docker](https://docs.docker.com/get-docker/)

   ```bash
   docker pull <your-dockerhub-username>/a5-stac-image

2. **Run the container:**
docker run -p 8888:8888 -v "$(pwd)":/app <your-dockerhub-username>/a5-stac-image

3. **Access JupyterLab:**

Copy the link displayed in the terminal and open it in your web browser.

4. **Execute the Notebook:**

Open s2_query.ipynb in JupyterLab and run the cells.

## Docker Image Details

- **Image Name**: a5-stac-image
- **Base Image**: contiuumio/miniconda:3.24.7.1-0
- **Installed Packages**:
  requests: 2.32.3
  pystac-client: 0.8.5
  matplotlib: 3.9.4
  jupyterlab: 4.3.4
  shapely: 2.0.6

