# Module 10: The Cloud Journey

[AWS Cloud Practitioner Home](https://github.com/pslucas0212/AWS-Cloud-Practioner)

### Introduction

AWS Well-Architeted Framework - analyze your architecture

#### Transcript
We've covered a lot of different AWS services in this course. And as you know, you use each individual service as building blocks for your solutions. There are endless architectures you can create to solve whatever problem you are trying to solve on AWS. You can string together services in a simple or complicated manner. Having a lot of options is great, but how do you know if the architecture you've created is, well, good? 

Let's look at this basic three-tier architecture. Does this look good? Well, we have a load balancer, some instances, and a backend database. Seems all right to me, but what about this alternate architecture? This architecture has now been replicated across Availability Zones or AZs. This is important for reliability. If one AZ is having issues, your application will still be up and running in the second AZ. It's important that you are able to spot deficiencies in architectures like in this simple example. 

Though not all examples are quite as simple. Luckily, there are tools that can help you get there. We're going to cover something called the Well-Architected Framework. This is a tool you can use to evaluate the architectures you build for excellence in a few different categories. The Well-Architected framework has pillars and these pillars are Operational Excellence, Security, Reliability, Performance Efficiency, and Cost Optimization.


### The AWS Well-Architected Framework

AWS Well-Archteted Framework is composed of 5 Pillars
- Operational excellence - monitor systems to improve 
- Security - 
- Reliability - Recovery planning and changes
- Performanc efficiency - using best Amazon EC2 type
- Cost optimization - optimize for money spent on AWS

Released AWS Well-Archteted Framework as a tool to use in evaluating your solution/architecture running on AWS

#### Transcript
The Well-Architected Framework is designed to enable architects, developers, and users of AWS to build secure, high-performing, resilient, and efficient infrastructure for their applications. It's composed of five pillars, to ensure a consistent approach to reviewing and designing of architectures. 

The first pillar is Operational Excellence. And focuses on running and monitoring systems to deliver business value, and with that, continually improving processes and procedures. For example, automating changes with deployment pipelines, or responding to events that are triggered. 

Second, is Security. And as you know, security is priority number 1 at AWS. And this pillar exemplifies it, by checking integrity of data and, for example, protecting systems by using encryption. 

Third, is Reliability. And it focuses on recovery planning, such as recovery from an Amazon DynamoDB disruption. Or EC2 node failure, to how you handle change to meet business and customer demand. 

Fourth, is Performance Efficiency, and it entails using IT and computing resources efficiently. For example, using the right Amazon EC2 type, based on workload and memory requirements, to making informed decisions, to maintain efficiency as business needs evolve. 

Lastly, we have Cost Optimization. Which looks at optimizing full cost. This is controlling where money is spent. And, for example, checking if you have overestimated your EC2 server size. You can then lower cost by choosing a more cost-effective size. 

In the past, you'd need to evaluate these against your AWS infrastructure with the help of a Solutions Architect. Not that you can't, and aren't still encouraged to do that, but we listened to customer feedback, and decided to release the Framework as a self-service tool, the Well-Architected Tool. You can access it by the AWS Management Console. Create a workload and run it against your AWS account. To generate a report, showing areas that should be addressed. 
It kinda looks like a traffic light system, with green being A-okay captain, keep up the good work. Orange being, you should probably look into this 'cause there's room for improvement. And red being, okay, you should look at this, 'cause something is at risk. These are areas where the tool has detected potential issues, and it presents you with a plan on how to architect, using established best practices. It should be noted that you can always override these settings if the questions don't apply to your scenario. It's very customizable. Interesting side note, where I'm from, South Africa, we call traffic lights robots. 

If we take a look at the tool itself, you'll see something similar to the following screenshot. As I mentioned, we name our workload and that appears in Section One. Section Two shows you the pillars and drop-downs into the questions for each. Section Three shows the actual questions themselves, Four is the pillar and question stem. Five is a bit of background, and the recommendation. Six is the answer you provide with a toggle to designate whether the question is applicable or not. This is important as it affects your overall score. Oh, and I can't forget Section Seven, where you'll be presented with short videos explaining how to answer a particular question. 

Anyhow, that's the Well-Architected Framework and tool. Hope you have enjoyed learning how to evaluate your workloads.

### Benefits of AWS Cloud

6 beneifts of using AWS cloud
1. Trade fixed expense for variable expense
2. Beneift from massive economies of scale - Acheive a lower variable cost
3. Stop guessing what capacity you need.  You could under or over estimate capacity to run your business
4. Increase Speed and Agility.  Easy to try new things and approaches.
5. Stop spending money on datacenters.  Focus on what makes your business different/better
6. Go global in minutes

#### Transcript
Alright, so now you've learned all there is to know about AWS and you're ready to go build your empire, right? Okay, so even if that isn't true you should still now have a good understanding of a lot of the different services AWS has to offer and how you can use them together like building blocks to build solutions for your business that scale, are flexible and are reliable. You also should by now understand some of the terminology AWS uses. Knowing this terminology is important for moving forward with your cloud journey. As you read blog posts or AWS documentation, you now should know a lot of the acronyms and phrases that you'll see. What you should also keep in mind as you move forward is the six main benefits of using the AWS Cloud. You'll start to evaluate what applications and solutions will be built in the Cloud. And knowing these benefits can really help you make those decisions in an informed way. Let's start with the first benefit.

This is a super important thing to remember. When you are building traditional on-premises data centers, you need to invest a large amount of money upfront just to get started. You need to invest cash into the actual data center physical space, all the hardware, the staff for racking and stacking that hardware and the overhead of keeping the data center running. For a medium to large business, this can be hundreds of thousands or millions of dollars. Then no matter what utilization is of that data center, you have a fixed cost and can set up your budget around that fixed cost. Billing with AWS is fundamentally different than the traditional billing model we just talked about. Your bill with AWS will be variable month to month as you consume more or less resources. Now the great thing about this is if you are just getting started there's no need to come up with a million dollars to invest into your AWS environment. Instead, you can start small, get billed for only what you use, and as you use more resources over time your bill will fluctuate with that growth. Now, if your bill gets out of your allotted budget, you can find ways to save money by turning off unused instances, deleting old resources that aren't being used, optimizing your applications, using tools like AWS Trusted Advisor to help you find opportunities to save money. Just because your bill was high one month, it doesn't mean you can't get it lowered the next month. And that's just not true with traditional on-premises data center billing. That's the first advantage. The next is

Benefit from massive economies of scale. This one is straight forward. AWS is building out massive amounts of capacity all around the world. And in order to build all those data centers, AWS is buying huge amounts of hardware. AWS is also an expert at building efficient data centers. We can buy the hardware at a lower price because of the massive volume, and then we install it and run it efficiently. Because of these factors, you can achieve a lower variable cost than you could running a data center on your own. Next up is

Stop guessing capacity. When you are building out a traditional data center, you need to estimate how much capacity you will need to run your business. Let's say you estimate you will have a user base of 10 million people over the next three years. You purchase enough hardware to support that growth over time and then turns out you only have about 500,000 users, much lower than you anticipated. Well, guess what? You are still stuck with that cost and hardware for the 10 million users. You overestimated your capacity. The other side of the coin here is that you estimate your capacity too low, and you now need to scramble to build out your data center, to handle the higher capacity before your customers have a degraded experience or before you lose customers altogether. That takes time and you most likely won't keep up, or you will have to put in a heroic effort to achieve it. Guessing your capacity upfront can be problematic if you either over or underestimate. With AWS, you don't need to guess your capacity. Instead, provision the resources you need for the now and then use the scaling mechanisms for each resource to scale up or down based on the real life capacity it needs from day to day as scaling can take minutes with AWS instead of weeks or months with on-premises resources. The next is my personal favorite benefit.

Increase speed and agility. With AWS, it's easy to try new things. You can spin up test environments and run experiments on new ways to approach solving a problem. And then if that approach didn't work, you can just delete those resources and stop incurring cost. Traditional data centers don't offer the same flexibility. And therefore, if you want to run an experiment that will require new servers being bought and installed, the cost of the experiment failing is high because you already bought the server. The flexibility of AWS helps drive innovation as well as the ease of provisioning resources. Getting a new database stood up on-premises might take weeks, in AWS, it takes minutes. That ability to quickly get the resources you need helps you get to market quicker. All right, next up.

Stop spending money running and maintaining data centers. If you aren't a data center company, why spend so much money and time running data centers? Let AWS take the undifferentiated heavy lifting off your hands and instead focus on what makes your business valuable. What makes your offering better than your competitors? AWS lets you focus on finding the answer to that and delighting your customers with new innovative solutions, instead of focusing on running hardware in a data center. And last but not least, we have.

Go global in minutes. Let's say you're a company based in the US and you want to expand your operations to Germany. You have data centers in the US serving this region but you'll need data centers in Germany to serve that region. Traditionally, you would need to have staff in Germany running and operating a data center for you. With AWS, you can just replicate your architecture to a region in Germany. And if you're set up correctly, you can do this in an automated fashion using tools like AWS CloudFormation. The time it takes for you to expand into a secondary area of the world traditionally can be months or years. With AWS, it just takes minutes.

That's it. Those are the six main benefits of using AWS. And from all of us at AWS, congratulations on completing the AWS Cloud Practitioner Essentials course.

If you want to dive even deeper, please check out our other course offerings for more information on AWS products and services.

And best of luck to you as you begin your cloud journey.
