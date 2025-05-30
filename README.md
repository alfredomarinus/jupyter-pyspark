# PySpark / Jupyter Notebook using Docker Compose

This repository provides a quick and easy way to launch a **Jupyter Notebook environment with PySpark**. It is designed to help you quickly set up a scalable data processing environment without complex local installations.

---

## Getting Started

Follow these steps to set up and access your PySpark-enabled Jupyter Notebook.

### Prerequisites

You only need **Docker Desktop** installed on your machine.
* [Download Docker Desktop](https://www.docker.com/products/docker-desktop)

### Running the Environment

1.  **Clone this repository** (or simply download the `docker-compose.yml` file into an empty directory):
    ```bash
    git clone https://github.com/alfredomarinus/jupyter-pyspark.git
    cd jupyter-pyspark
    ```

2.  **Start the Docker services:**
    Open your terminal in the directory where `docker-compose.yml` is located and run:
    ```bash
    docker-compose build --no-cache
    docker-compose up --d
    ```
    This command will download the necessary Docker images (if not already present) and start the Jupyter Notebook server.

### Accessing Jupyter Notebook

Once the services are running (you will see a lot of output in your terminal), open your web browser and go to:

`http://127.0.0.1:8888`


---

## What is Included

The `docker-compose.yml` file sets up a Jupyter Notebook environment with:

* **PySpark:** For distributed data processing.
* **Python:** The language for your notebooks.
* **Jupyter Notebook/Lab:** For interactive development.