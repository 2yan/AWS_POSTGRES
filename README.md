# AWS Lambda Layers Library

## Overview
This repository contains prebuilt Lambda Layers for AWS, including PostgreSQL connectors and popular Python libraries.

## Available Layers

### PostgreSQL Connectors
- **psycopg2** layers for Python 3.8-3.12
- **psycopg3** layers for Python 3.8-3.12

### Additional Libraries
- **Facebook Prophet** - Time series forecasting library
- **Jinja2** - Template engine for Python
- **OpenAI** - Official OpenAI Python library
- **Tableau Server Client** - Python client for Tableau Server API
- **Ulysses** - Custom utility library

## Features
- **Ease of Use**: Attach the layer to your Lambda function
- **Seamless Integration**: Ready-to-use Python libraries in AWS Lambda
- **Multiple Python Versions**: Support for Python 3.8-3.12

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
   # PostgreSQL connections
   import psycopg2
   # OR
   import psycopg
   
   # Other libraries
   import openai
   from prophet import Prophet
   import jinja2
   import tableauserverclient
   
   # Now you can use these libraries in your Lambda function
