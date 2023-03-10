# Week 1 — App Containerization

## homwork

### Containerize Application

#### backend-flask
i edited the dockerfile to leverage multi-stage builds. This has allowed me slim down the image size from 129 MB to 122 MB (image for proof)

![multi-stage build Dockerfile](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/multi-stage%20build.PNG)

running container:

![running container](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/running_container.PNG)

#### frontend
as a DevOps engineer who has done this at work, i builf the reactjs app and set it up to be served via nginx. I have also leveraged multi-stage builds to slim down the size of this image. The configuration file for nginx used in the Dockerfikle can be found under the directory. note that since this is being served thru nginx the port of the container is 80.

![image](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/react_image_size.PNG)

screenshot:

![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/fe_prof.PNG)

#### docker-compose

![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/docker-composer.PNG)

as you can see running docker compose with my own fancy nginx image did not work and gave me the following error:


![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/weird_error)

so i defaulted to the dockerfile provided in this bootcamp. I kept my own "fancy" dockerfile and will try to makw it work at some point in the future.

![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/composer_final.PNG)





### Snyk Integration

![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/snyk_integration.PNG)

### Notifications


#### front-end    
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/notifs_fe.PNG)    

#### back-end    
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/notifs_be.PNG)  




