source venv/Scripts/activate   

# AQIweb

A Multimodal AQI prediction model

## How to Run the Full Backend

1. The stable version is located in the `main` branch.
2. Navigate to the project directory:
    
    ```bash
    cd VQAweb
    
    ```
    
3. Modify the file `VQAweb/frontend/Present/src/components/Pictureinput.vue`:
    
    Replace `localhost` in the `axios.post` line with your `<server_IP>`.
    
4. Run the backend using the following script:
    
    ```bash
    ./docker_run.sh
    
    ```
    
    If you encounter execution issues, make the script executable first:
    
    ```bash
    chmod +x ./docker_run.sh
    ./docker_run.sh
    
    ```
    
5. Access the application in your browser:
    
    Visit `<server_IP>:8000` in your web browser.
    
6. To stop the application:
    
    Press `Ctrl + C` in the terminal.
    
    **Note:**
    
    If Docker images are not successfully deleted, manually modify the `docker rmi` command in the `./docker_run.sh` script to remove them.
