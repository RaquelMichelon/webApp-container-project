# Web App Container

This project uses Docker Compose to run an HTML aplication in an Apache Container.

Steps

## 1 Create an YML file defining an Apache server (httpd); 

## 2 Especify in the YML file where the aplication files will be; 

As especified on volumes, the aplication files should be on `/website` directory.

  ````
  
   volumes:
    - ./website:/usr/local/apache2/htdocs
    
  ````
  
  `mkdir website` to create the folder and `cd website` to access the folder
  
  `nano index.html` to create a simple html file (Apache will run html, css and js files)
  
  `cd .. ` to go back to previous directory
  
  `apt install docker-compose` to install docker compose
  
  `docker-compose up -d` and `docker container ls` - to up the conteiner and verify if is running
  
  The app will be running on the hostIP:80
  
  
## 3 Upload the YML and the app into a GitHub repo
