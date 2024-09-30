
### REMINDER
# Proyecto AWS_SAAC-003

Este repositorio contiene código y recursos relacionados con el curso **AWS Certified Solutions Architect - Associate (SAA-C03)** impartido por **Adrian Cantrill**. Todo el contenido de este repositorio ha sido creado siguiendo su curso y las instrucciones proporcionadas en el mismo.

## Autoría

El código y las ideas reflejadas en este repositorio pertenecen completamente a **Adrian Cantrill**, quien ha desarrollado el contenido de manera original a través de su curso.

### Curso de Adrian Cantrill en AWS Certified Solutions Architect - Associate (SAA-C03)

Para más información o para acceder al curso, puedes visitar los siguientes enlaces:

- [AWS Certified Solutions Architect - Associate (SAA-C03) en AdrianCantrill.com](https://learn.cantrill.io/p/aws-certified-solutions-architect-associate-saa-c03)
- [AWS Certified Solutions Architect - Associate (SAA-C03) en Udemy](https://www.udemy.com/course/aws-certified-solutions-architect-associate/)

Agradecimientos especiales a Adrian Cantrill por compartir su conocimiento y contribuir al éxito de quienes buscan certificarse en AWS.

## Uso del Repositorio

Este repositorio se utiliza con fines educativos siguiendo las directrices del curso de **Adrian Cantrill**. Se recomienda no utilizar el contenido con fines comerciales ni distribuirlo sin la debida atribución.

---

# AWS_SAAC-003 Project

This repository contains code and resources related to the **AWS Certified Solutions Architect - Associate (SAA-C03)** course taught by **Adrian Cantrill**. All the content in this repository has been created following his course and instructions.

## Attribution

The code and ideas reflected in this repository fully belong to **Adrian Cantrill**, who originally developed the content through his course.

### Adrian Cantrill's AWS Certified Solutions Architect - Associate (SAA-C03) Course

For more information or to access the course, you can visit the following links:

- [AWS Certified Solutions Architect - Associate (SAA-C03) on AdrianCantrill.com](https://learn.cantrill.io/p/aws-certified-solutions-architect-associate-saa-c03)
- [AWS Certified Solutions Architect - Associate (SAA-C03) on Udemy](https://www.udemy.com/course/aws-certified-solutions-architect-associate/)

Special thanks to Adrian Cantrill for sharing his knowledge and contributing to the success of those seeking AWS certification.

## Repository Usage

This repository is used for educational purposes following the guidelines of **Adrian Cantrill's** course. It is recommended not to use the content for commercial purposes or distribute it without proper attribution.


### Advanced Demo - Web App - Single Server to Elastic Evolution

In this advanced demo lesson you are going to evolve the architecture of a popular web application wordpress
The architecture will start with a manually built single instance, running the application and database
over the stages of the demo you will evolve this until its a scalable and resilient architecture

The demo consists of 6 stages, each implementing additional components of the architecture  

- Stage 1 - Setup the environment and manually build wordpress  
- Stage 2 - Automate the build using a Launch Template  
- Stage 3 - Split out the DB into RDS and Update the LT 
- Stage 4 - Split out the WP filesystem into EFS and Update the LT
- Stage 5 - Enable elasticity via a ASG & ALB and fix wordpress (hardcoded WPHOME) 
- Stage 6 - Cleanup  

![Architecture](https://github.com/acantril/learn-cantrill-io-labs/raw/master/aws-elastic-wordpress-evolution/ArchitectureEvolutionAll.png)

## Instructions

- [Stage1](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE1%20-%20Setup%20and%20Manual%20wordpress%20build.md)
- [Stage2](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE2%20-%20Automate%20the%20build%20using%20a%20Launch%20Template.md)
- [Stage3](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE3%20-%20Add%20RDS%20and%20Update%20the%20LT.md)
- [Stage4](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE4%20-%20Add%20EFS%20and%20Update%20the%20LT.md)
- [Stage5](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE5%20-%20Add%20an%20ELB%20and%20ASG.md)
- [Stage6](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE6%20-%20CLEANUP.md)


## 1-Click Installs
Make sure you are logged into AWS and in `us-east-1`  

- [VPC](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/quickcreate?templateURL=https://learn-cantrill-labs.s3.amazonaws.com/aws-elastic-wordpress-evolution/A4LVPC.yaml&stackName=A4LVPC)

## Video Guides

- [HERE](https://youtu.be/wWIFJvxoWb0)


## Architecture Diagrams

- [Stage1 - PNG](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE1%20-%20SINGLE%20SERVER%20MANUAL.png)
- [Stage1 - PDF](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE1%20-%20SINGLE%20SERVER%20MANUAL.pdf)
- [Stage2 - PNG](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE2%20-%20SINGLE%20SERVER%20LT.png)
- [Stage2 - PDF](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE2%20-%20SINGLE%20SERVER%20LT.pdf)
- [Stage3 - PNG](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE3%20-%20SPLIT%20OUT%20RDS.png)
- [Stage3 - PDF](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE3%20-%20SPLIT%20OUT%20RDS.pdf)
- [Stage4 - PNG](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE4%20-%20SPLIT%20OUT%20EFS.png)
- [Stage4 - PDF](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE4%20-%20SPLIT%20OUT%20EFS.pdf)
- [Stage5 - PNG](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE5%20-%20ASG%20%26%20ALB.png)
- [Stage5 - PDF](https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-elastic-wordpress-evolution/02_LABINSTRUCTIONS/STAGE5%20-%20ASG%20%26%20ALB.pdf)






