# Udagram Image Filtering Microservice

## Development Branch

    f-filter

## Run locally

    npm run dev

## Build command

    npm run build

## Deployed to ELB
Deployed to Elasticbeanstalk using following steps:

Initialised and created elb environment

    elb init

    elb create

Added to .elasticbeanstalk/config.yml

    deploy:
        artifact: ./www/Archive.zip

Deployed

    elb deploy

Endpoint URL: http://image-filter-dev.ap-southeast-2.elasticbeanstalk.com/filteredimage?image_url={{url}}

Working example: http://image-filter-dev.ap-southeast-2.elasticbeanstalk.com/filteredimage?image_url=https://cnet3.cbsistatic.com/img/zAmm1HM_kG-FjQa5YPMShKiM8_I=/2018/04/25/0c1edd36-e90b-42bc-abc6-e8fcfc2395a9/iron-man-2.jpg
