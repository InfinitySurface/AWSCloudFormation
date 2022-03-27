# CloudFormation

CloudFormation is an AWS service that uses files (.json/.yaml) to deploy resources across the AWS infrastructure. CloudFromation is essential for many developers that helps productivity, time, and even cost when developing big cloud projects for a company. You will be able to download the given sample .yaml files and deploy them yourself on CloudFormation!

<p align="center">
  <img src="https://user-images.githubusercontent.com/98137377/159177689-c6e65174-002c-4646-83bf-c4b27d7f9b64.png">
</p>

## Table Of Contents

- [About The Project](#about-the-project)
    - [Flowchart](#flowchart)
    - [Built With](#built-with)
- [Getting Started](#getting-started)
    - [Accessing CloudFormation](#accessing-cloudformation)
    - [Create Stack](#create-stack)
    - [Stack Prerequisite](#stack-prerequisite)
    - [Stack Details](#stack-details)
    - [Stack Creation](#stack-creation)
- [Navigation](#navigation)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

## About The Project

### Flowchart

![CloudFormation Flowchart (1)](https://user-images.githubusercontent.com/98137377/159145487-fe0ee9cf-fa55-4620-97ca-3aab776be2ac.png)

</p>
<p align = "center">
Flow Chart Built with LucidChart
</p>

This flowchart represents the infrastructrue of how the 3 .yaml files will deploy a dummy application on a webserver running on an EC2 instance. The network.yaml file will deploy a VPC, with a pair of public and private subnets that spread across two Availabilty Zones. It deploys an Internet Gateway, with a default route on the public subnets. It then deploys a pair of NAT Gateways in the two avalability zones and defaults them to the private subnets. The serversecurity.yaml will deploy our two servers for our application while setting up security groups for both. Lastly, the storagedatabase.yaml file deploys 2 databases for our dummy application.

### Built With

The database.yaml file was editited with the built in AWS CloudFormation Template Designer.

The CloudFormation Flowchart was created on Lucidchart.

## Getting Started

There are many ways of deploying your .yaml files to construct the infrastructure above. For instance you can use your local SSH or just going right through AWS itself. For this case we will be using AWS to deploy our files.

### Accessing CloudFormation

To get started, make sure you have an AWS account created and the 3 given .yaml files to deploy on CloudFormation.

Then proceed to your AWS dashboard and search for CloudFormation on the search bar.

![Dashboard](https://user-images.githubusercontent.com/98137377/159184215-8ab5970d-f348-458d-8aaf-03dce22e4842.jpg)

![Search](https://user-images.githubusercontent.com/98137377/159184216-30d725f3-390c-4d2f-a6d2-3a8230a12b42.jpg)

### Create Stack

When you make it to the CloudFront Dashboard, you will need to create a new Stack.

A stack is essentially a collection of resources in a file (.json/.yaml) that you can manage as a single unit.

![stackDash](https://user-images.githubusercontent.com/98137377/159184542-d4124cc3-769c-47ae-8ac3-bfbecf780fae.jpg)

### Stack Prerequisite

![stack creation](https://user-images.githubusercontent.com/98137377/159184814-4fac884b-1a61-46da-889d-3e8e5b7757d1.jpg)

Once you've clicked on 'Create stack', you will be taken to this page.

The 'Stack Prerequisite' page offers the user how they would like to prepare their template. In this case, we will select 'Template is ready" option since we already have our premade .yaml files.

AWS does offer 2 other ways that lets you prepare a template, Sample Template and Template Designer:

* Sample Templates:  premade stacks that you can deploy.

* Template Designer: graphically design your stack on a grid with all avaliable AWS resources at your disposal. 

Once you also selected the option 'Upload a template file, and the desired .yaml file to upload, click 'Next'.

***Note: You can only upload a file one at at time, so repeat these steps for when you are ready to upload the other two files.***

### Stack Details

![stackdetails](https://user-images.githubusercontent.com/98137377/159185136-187e9deb-e3e2-455e-ae8d-4229e861be9e.jpg)

On this page 'Specify Stack Details', this is where you will give a name to this stack as well as filling in any parameter if given.

Paramters are how you can customize your AWS Infrastructures through the .yaml files. For example, the 'AMItoUse' shown above allows the user to input which AMI they decide to use instead of having it hardcoded in the .yaml file. This is key to efficency as this will make updating an specific AWS Infrastructrue much easier and faster instead of always hardcoding the value in the .yaml file.

Once you have given the stack a name and filled out all (if any) parameters, click 'Next'.

***Note: Step 3 can be skipped since we don't really have to change any stack options so you can skip straight to Step 4 and 'Create stack'.*** 

### Stack Creation

![last](https://user-images.githubusercontent.com/98137377/159185296-21d06d18-dfca-4ecb-a744-881c65e68292.jpg)

After you selected 'Create Stack', CloudFormation will then read your .yaml file and start deploying each AWS resource over a course of a couple minutes.

To check if CloudFormation has fully created all of your resources, you can check the status on the left to show if the stack has completed its deployment.

***Note: Deployment time can vary depending on the complexity of your .json/.yaml files you are uploading.***

## Navigation

![image](https://user-images.githubusercontent.com/98137377/159185376-dd4a2cfc-c185-4bf9-a323-dbf0d54f8113.png)

You can manage all your created stacks by accessing CloudFormation->Stacks.

The stacks dashboard will give you insights on your stack such as when the stack was created or a breif description of your stack.

The dashboard also allows you to update, delete, and create another stack if you wish to do so.

## License

This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details

## Contact

Name: Anthony G. Surface

Personal Email: tonysurface200@gmail.com

University Email: anthony.surface@my.utsa.edu

Github Profile: https://github.com/InfinitySurface

## Acknowledgments

Resources Used:

* [AWS](https://aws.amazon.com/?nc2=h_lg)
* [LucidChart](https://www.lucidchart.com/pages/)
