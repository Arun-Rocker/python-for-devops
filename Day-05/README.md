Environment variables are a fundamental way to configure applications without hardcoding sensitive or environment-specific values. 
Here's a comprehensive guide to working with environment variables in Python.

## Linux/macOS:

using below command we should export env variable to linux/mac
```
export DB_HOST="localhost"
```

In the code we call env variable by using `os.getenv`
```
import os

## ** Simple get with optional default **
api_key = os.getenv('API_KEY', 'default-key')
```
