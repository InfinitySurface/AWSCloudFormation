# CloudFormation using AWS

CloudFormation is an AWS service that uses files (.json/.yaml) to deploy resources across the AWS infrastructure. CloudFromation is essential for many developers that helps productivity, time, and even cost when developing big cloud projects for a company. You will be able to download the given sample .yaml files and deploy them yourself on CloudFormation!

<p align="center">
  <img src="https://user-images.githubusercontent.com/98137377/159177689-c6e65174-002c-4646-83bf-c4b27d7f9b64.png">
</p>

## Table Of Contents

- [About The Project](#about-the-project)
    - [Flowchart](#flowchart)
    - [Flowchart Breakdown](#flowchart-breakdown)
    - [Built With](#built-with)
- [Getting Started](#getting-started)
    - [Deploying the YAML Files](#deploying-the-yaml-files)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

## About The Project

### Flowchart

Below is a flowchart that represents the dummy application we will be deploying on CloudFormation from the .yaml files.

![CloudFormation Flowchart (1)](https://user-images.githubusercontent.com/98137377/159145487-fe0ee9cf-fa55-4620-97ca-3aab776be2ac.png)

</p>
<p align = "center">
Flow Chart Built with LucidChart
</p>

### Flowchart Breakdown



### Built With

All 3 .yaml files were editited with the built in AWS CloudFormation Designer.

The CloudFormation Flowchart was made on Lucidchart.

## Getting Started

### Accessing CloudFormation

To get started, make sure you have an AWS account created and the 3 given .yaml files to deploy on CloudFormation.

Then proceed to your AWS dashboard and search for CloudFormation on the search bar.

![Dashboard](https://user-images.githubusercontent.com/98137377/159184215-8ab5970d-f348-458d-8aaf-03dce22e4842.jpg)

![Search](https://user-images.githubusercontent.com/98137377/159184216-30d725f3-390c-4d2f-a6d2-3a8230a12b42.jpg)

### Deploying the YAML Files - Create Stack

When you make it to the CloudFront Dashboard, you will need to create a new Stack.

A stack is essentially a collection of resources in a file (.json/.yaml) that you can manage as a single unit.

![stackDash](https://user-images.githubusercontent.com/98137377/159184542-d4124cc3-769c-47ae-8ac3-bfbecf780fae.jpg)

### Deploying the YAML Files - Stack Prerequisite

Once you've clicked on 'Create stack', you will be taken to this page.

![stack creation](https://user-images.githubusercontent.com/98137377/159184814-4fac884b-1a61-46da-889d-3e8e5b7757d1.jpg)

The 'Stack Prerequisite' page offers the user how they would like to prepare their template. In this case, we will select 'Template is ready" option since we already have our premade .yaml files.

AWS does offer 2 other ways that lets you prepare a template, Sample Template and Template Designer:

* Sample Templates:  premade stacks that you can deploy.

* Template Designer: graphically design your stack on a grid with all avaliable AWS resources at your disposal. 

Once you also selected the option 'Upload a template file, and the desired .yaml file to upload, click 'Next'.

***Note: You can only upload a file one at at time, so repeat these steps for when you are ready to upload the other two files.***

### Deploying the YAML Files - Stack Details

![stackdetails](https://user-images.githubusercontent.com/98137377/159185136-187e9deb-e3e2-455e-ae8d-4229e861be9e.jpg)

![last](https://user-images.githubusercontent.com/98137377/159185296-21d06d18-dfca-4ecb-a744-881c65e68292.jpg)

![image](https://user-images.githubusercontent.com/98137377/159185376-dd4a2cfc-c185-4bf9-a323-dbf0d54f8113.png)

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
