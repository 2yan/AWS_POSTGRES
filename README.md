# AWS Lambda Layers Library

## Overview
This repository contains prebuilt Lambda Layers for AWS, including PostgreSQL connectors and popular Python libraries.

## Available Layers

### PostgreSQL Connectors
- **psycopg2-binary v2.9.9** layers for Python 3.8-3.12
- **psycopg v3.1.18** layers for Python 3.8-3.12

### Additional Libraries
- **Facebook Prophet v1.1.5** - Time series forecasting library (Python 3.9)
- **Jinja2 v3.1.2** - Template engine for Python (with MarkupSafe v2.1.3)
- **OpenAI v0.28.0** - Official OpenAI Python library (Python 3.9)
- **Tableau Server Client v0.28** - Python client for Tableau Server API (Python 3.9)
- **Ulysses** - Microsoft SQL Server connectivity library (numpy v1.26.1, pandas v2.1.1, pyodbc v4.0.26)

## Layer Details

| Layer Name | Python Version | Library Version | Description |
|------------|----------------|-----------------|-------------|
| **psycopg2_3.8.zip** | 3.8 | psycopg2-binary v2.9.9 | PostgreSQL adapter for Python 3.8 |
| **psycopg2_3.9.zip** | 3.9 | psycopg2-binary v2.9.9 | PostgreSQL adapter for Python 3.9 |
| **psycopg2_3.10.zip** | 3.10 | psycopg2-binary v2.9.9 | PostgreSQL adapter for Python 3.10 |
| **psycopg2_3.11.zip** | 3.11 | psycopg2-binary v2.9.9 | PostgreSQL adapter for Python 3.11 |
| **psycopg2_3.12.zip** | 3.12 | psycopg2-binary v2.9.9 | PostgreSQL adapter for Python 3.12 |
| **psycopg3_3.8.zip** | 3.8 | psycopg v3.1.18 | Modern PostgreSQL adapter for Python 3.8 |
| **psycopg3_3.9.zip** | 3.9 | psycopg v3.1.18 | Modern PostgreSQL adapter for Python 3.9 |
| **psycopg3_3.10.zip** | 3.10 | psycopg v3.1.18 | Modern PostgreSQL adapter for Python 3.10 |
| **psycopg3_3.11.zip** | 3.11 | psycopg v3.1.18 | Modern PostgreSQL adapter for Python 3.11 |
| **psycopg3_3.12.zip** | 3.12 | psycopg v3.1.18 | Modern PostgreSQL adapter for Python 3.12 |
| **facebook_prophet.zip** | 3.9 | prophet v1.1.5 | Time series forecasting library |
| **jinja2.zip** | 3.9 | jinja2 v3.1.2 | Template engine for Python |
| **openai.zip** | 3.9 | openai v0.28.0 | Official OpenAI Python library |
| **tableau_server_client.zip** | 3.9 | tableauserverclient v0.28 | Python client for Tableau Server API |
| **ulysses.zip** | 3.9 | Custom | Microsoft SQL Server connectivity (numpy, pandas, pyodbc) |

## Features
- **Ease of Use**: Attach the layer to your Lambda function
- **Seamless Integration**: Ready-to-use Python libraries in AWS Lambda
- **Multiple Python Versions**: Support for Python 3.8-3.12
- **Version Tracking**: All layers include detailed version information

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
