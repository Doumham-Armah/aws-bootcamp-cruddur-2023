# Week 2 — Distributed Tracing.   

### Honeycomb.   

![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/honeycomb_integration.png) 

### AWS X-Ray   
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/x-ray_segments_proof.PNG)    
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/x-ray%20group_in_aws.PNG)     
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/x-ray%20group.PNG)    
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/trace_proof_aws_console.PNG)    
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/sampling_rule_xray.PNG)   

#### X-Ray subsegments    
i thought this was left out from hw but then realized after i submitted the hw that andrew made a vidoe to fix it so i followed along and got it fixed too!    
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/mock_data.PNG) 

#### Error
The aws_default _region env variable is not being transferred over to the daemon container so i had to hardcode it in the docker compose file as shown below:    
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/aws_def_region.PNG)    

### CloudWatch Logs    
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/cloudwatch_proof.PNG)    

### Rollbar  
![ss](https://github.com/Doumham-Armah/aws-bootcamp-cruddur-2023/blob/main/journal/assets/rollbar_integration_proof.png)    
