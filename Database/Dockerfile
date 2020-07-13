FROM mysql 

RUN apt-get update
RUN apt-get install vim iputils-ping -y

  
# Environment variables - Set root password and create a db 

ENV MYSQL_ROOT_PASSWORD ampsql123
  

ENV MYSQL_DATABASE ampdb 

  

  

# Add the content of the init/ directory to your image 

# # All scripts in docker-entrypoint-initdb.d/ are automatically 

# # executed during container startup 


COPY ./init/ /docker-entrypoint-initdb.d/ 
