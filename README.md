# Cloud Journey Docker Compose Configuration

## Overview

This Docker Compose configuration sets up a Python application using Django. The "app" service builds and runs the application within a Docker container.

## Quick Start

1. **Clone the repository:**

   ```
   git clone https://github.com/your/repository.git
   cd your-repository
   ```

1. **Customize the application code:**

Place your Python application source code in the src directory.

2. **Build and run the Docker container:**
 ```
 docker-compose up --build
 ``` 
 Access the application at http://localhost:8000.
 

## Configuration Details

Services
**`app`**
**Build:** Docker image from **`src`**.
**Command:** **python manage.py runserver** **`0.0.0.0:8000`**.
**Volumes:** **`./src:/app`** for live code updates.
**Ports:** Exposed on **`8000`**, mapped to host's **`8000`**.