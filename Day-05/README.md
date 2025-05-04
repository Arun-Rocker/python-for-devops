Environment variables are a fundamental way to configure applications without hardcoding sensitive or environment-specific values. 
Here's a comprehensive guide to working with environment variables in Python.

## Linux/macOS:

using below command we should export env variable to linux/mac
```
# Add to ~/.bashrc, ~/.zshrc, or ~/.profile
export API_KEY="your_api_key_here"
export DB_HOST="localhost"
```

In the code we call env variable by using `os.getenv`
```
import os

# Method 1: os.environ (raises KeyError if missing)
api_key = os.environ['API_KEY']

# Method 2: os.getenv() (safer, returns None if missing)
db_host = os.getenv('DB_HOST')

# Method 3: With default value
db_port = os.getenv('DB_PORT', '5432')  # Default to 5432 if not set
```
