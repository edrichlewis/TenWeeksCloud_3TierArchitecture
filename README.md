# TenWeeksCloud_3TierArchitecture
Three-Tier Architecture to Host Web Application in AWS

![Project2 Presentation](https://github.com/edrichlewis/TenWeeksCloud_3TierArchitecture/assets/105597780/babd4108-e5cb-43be-8215-f64d2d5b058c)


This is an animated architecture diagram for hosting 3 tier architecture
The details about learning and the required steps to create this architecture are provided in the Link: https://catalog.us-east-1.prod.workshops.aws/workshops/85cd2bb2-7f79-4e96-bdee-8078e469752a/en-US/introduction

After following the above steps we create a cloud-front Distribution CDN
![image](https://github.com/edrichlewis/TenWeeksCloud_3TierArchitecture/assets/105597780/b0e9721f-40dc-4e39-b6cb-58a0ca7c6902)

Enter the origin domain as WebTierLoadBalancer, and select the protocol as HTTP
Keep the default settings and if we need to input details into the DB using UI we have to select the allowed HTTP methods as GET, HEAD, OPTIONS, PUT, POST, PATCH, DELETE 
![image](https://github.com/edrichlewis/TenWeeksCloud_3TierArchitecture/assets/105597780/77670a36-f76b-4bf1-a4ea-c08dfd08645b)

Enable WAF security protection, keep the default settings, and request an SSL certificate 

select the radio button to request a public certificate, Enter the registered domain name, select the DNS validation and click on Request.

For detailed steps we can follow the steps from "Step 4" from the given Repo: https://github.com/edrichlewis/TenWeeksCloud_static_s3, to create a distribution and configure the Domain name in NameCheap.

once we complete the above steps we can access the Website via the Domain name in this case https://wwww.edrich.store  (this service is deleted after the completion of the Project)

![image](https://github.com/edrichlewis/TenWeeksCloud_3TierArchitecture/assets/105597780/0c515528-2587-45ce-8591-2931a022f7c4)

![image](https://github.com/edrichlewis/TenWeeksCloud_3TierArchitecture/assets/105597780/88bd5fee-9512-46d4-837c-e1ad08907739)

