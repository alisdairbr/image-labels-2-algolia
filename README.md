# Information to write the tutorial


## What is this example about?

This demo showcase how to use Koyeb, Algolia and Fastly to create an application that detect labels on images using AWS Rekognition, index these labels into Algolia and make them searchable for the end user

## What is required to successfully execute this tutorial

- Koyeb account
- Fastly account for CDN
- Algolia account to index and search images
- NextJS app to let user upload and explore images (Not done yet)

## How this function works

This function is a Node.js function which is triggered by a store event. We filter events with object key extension `PNG` and `JPG`

## What I need to do to use and run the app

You need to create:

- An algolia index
- AWS Credentials to access AWS Rekognition
- A Koyeb store to upload and retrieve files
- A Fastly account and a new service to serve your content
- 5 secrets into Koyeb
  - aws-access-key containing your aws access key to access rekognition service
  - aws-secret-key containing your aws secret key to access rekognition service
  - algolia-app-id containing your algolia app id
  - algolia-api-key containing your algolia api key
  - algolia-index containing your algolia index

  ## How to deploy this Stack?

  Fork this repository, edit variables in koyeb.yaml file with your own

