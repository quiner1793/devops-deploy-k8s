# Variables

## Generate DOCKER_CREDS

1. For your docker registry:

```shell
echo -n "your_username:your_password" | base64
```

2. Create the JSON Structure

Form the DOCKER_CREDS file:  
   
```
{
    "auths": {
        "https://index.docker.io/v1/": {
            "auth": "YOUR_BASE64_ENCODED_CREDENTIALS"
        }
    }
}
```
