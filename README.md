# AWS PostgreSQL Lambda Layer 
Disclaimer:  I had AI help with this readme but it is overall appropriate, concise and has better grammar than I would normally have. 

## Overview
This repository contains prebuilt PostgreSQL Lambda Layers for AWS.

## Features
- **Ease of Use**: Attach the layer to your Lambda functio..
- **Seamless Integration**: Allows you to use `psycopg2` or `psycopg3` to interact with your PostgreSQL database.

## Getting Started
1. **Upload the Lambda Layer**:
   - Navigate to the AWS Lambda Management Console.
   - Choose "Layers" from the left-hand menu.
   - Select "Create layer", and upload the provided layer package, the names of the packages corrospond to the python version they support.

2. **Attach the Layer to Your Lambda Function**:
   - Open your Lambda function in the AWS Console.
   - In the "Layers" section, choose "Add a layer".
   - Select the uploaded PostgreSQL under custom layers and add it to your function.

3. **Use in Your Application**:
   ```python
   import psycopg2
   OR
   import psycopg
   # Now, you can establish a connection to your PostgreSQL database and execute SQL statements as usual.
