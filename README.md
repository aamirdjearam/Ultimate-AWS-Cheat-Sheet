# Ultimate-AWS-Cheat-Sheet

## Objective

  The Ultimate AWS Cheat Sheet is a wordpress Website hosted on Amazon Elastic Compute Cloud. The objective of this project is to host the website completely using AWS services for as little as possible. The project should adhere to the core principles of the AWS Well-Architected Principles but should prioritize cost-optomization. We will architect several different solutions and then choose the most appropriate path depending on what the customer values.
  
  This Readme will be seperated into several different sections
  
1. Planning phase

2. T2 Vs T3 Micro (Which is the better use case) 

3. Lightsail

4. EC2 (Using Wordpress AMI)

5. Route 53

6. Analysis

7. Conclusion
  
  
# Planning Phase

Due to time constraints, creating a custom website utilizing HTML, CSS & Javascript was not a possibility, so we began to look for alternatives. **Wordpress was ultimately chosen as an alternative as it was inexpensive, flexible with AWS and easy to use.** Amazon has already posted a whitepaper regarding how to install Wordpress using Amazon Lightsail however we would also like to make this available on all Availability Zones. Currently the Wordpress Lightsail Instance is unavailable in the US West region (US WEST-1 N. California) and while the latency difference wouldn't particularly be noticable. 

We will try multiple methods and calculate the cost, performance, scalability and availability. 

For Test Instances we will utilize a dummy site with dummy data using the ["Demo Data Creator Plugin"](https://wordpress.org/plugins/demo-data-creator/) 

# T2 VS T3 (Micro)

Part of architecting any solution on AWS should start with estimating Hardware Requirements as the first step as this dictates the majority of the pricing for this project. For running a Wordpress instance (with most likely less than 500 visitors per month) a single core (micro) chip 

