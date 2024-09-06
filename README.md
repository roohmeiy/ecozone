# ecozone
This website provides information about clean energies. It is build using html,css and javascript.

## Installation and Setup

Follow these steps to deploy this website using Nginx on an Ubuntu server.
1.  Update your system install and start Nginx:
   ```bash
   sudo apt update
   sudo apt install nginx
  sudo systemctl start nginx
```
2. Clone the repository and cd 
   ```
   git clone https://github.com/roohmeiy/ecozone.git
   cd ecozone/
   ```
3.. Move the project files to the web server directory:
```bash
sudo mv /path to/ecozone /var/www/
```

4. Configure Nginx to serve the website:
  ```bash
   sudo vi /etc/nginx/sites-available/default
   ```
   Update the root directive in the server block:
   
   ```bash
   root /var/www/ecozone;
   ```

5. Test the Nginx configuration:
  ```bash
  sudo nginx -t
  ```

6. If the test is successful, reload Nginx to apply the changes:
  ```bash
sudo systemctl reload nginx
```
7. Access the Project once the setup is complete, you should be able to access the ecozone project by navigating to your server's IP address in a web browser.
   ```bash
   http://localhost:80
```



