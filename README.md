![Group 16](https://github.com/MohyiddineDilmi/GraphiaX/assets/33746487/796f0274-c84a-4110-b9ee-b224af59f355)

#

GraphiaX is a groundbreaking tool designed to enhance code understanding and streamline developer onboarding! By transforming code into graphs, developers can now visualize and comprehend complex structures with ease. You can simply enter the repository URL link, and the code is transformed into an intuitive graph representation.

## Supported Language 
`React`

Live Demo: https://graphiax.azurewebsites.net/

# Architecture

Frontend `React JS`,
Backend `Django`,
Host `Azure Web Service`

<img src="https://github.com/MohyiddineDilmi/GraphiaX/assets/33746487/9329de75-42f3-4915-b003-5b863c56b112" width="20%"/>

# Frontend

Repo Link: https://github.com/MohyiddineDilmi/graphiax-frontend

GraphiaX Frontend Docker image: 
https://hub.docker.com/repository/docker/dilmi0000/graphiax-frontend/general

## Important
```JS
// 1 - Go to Home.jsx file
// 2 - Replace BASE_URL with your server URL
const BASE_URL = 'Your Server URL';
// In our case BASE URL == https://graphiax-server.azurewebsites.net
BASE_URL = 'https://graphiax-server.azurewebsites.net';
const url = `${BASE_URL}/react_api/info/`;
```

>💡 We will focus more on the backend.

# Backend

Repo Link: https://github.com/MohyiddineDilmi/graphiax-server

## Requirements

```
asgiref==3.7.2
certifi==2023.7.22
charset-normalizer==3.2.0
Django==4.2.3
django-cors-headers==4.2.0
gunicorn==21.2.0
idna==3.4
packaging==23.1
requests==2.31.0
sqlparse==0.4.4
tzdata==2023.3
urllib3==2.0.4
```

## Server Architecture

* One endpoint `(GET)  BASE_URL/react_api/info/`
* For the communication with the GitHub repo, we used [GitHub Api Repository contents](https://docs.github.com/en/rest/repos/contents?apiVersion=2022-11-28)

<img src="https://github.com/MohyiddineDilmi/GraphiaX/assets/33746487/4d4e3b46-d3b4-425d-9d5d-52e2ac6f3ee3" width="70%"/>

## Important
```python
# 1 - Go to utils.py file
# 2 - Replace access_token with your github token
access_token = 'your_github_token_here'
```

```python
# 1 - Go to settings.py file
# 2 - Add your frontend url in CORS_ALLOWED_ORIGINS
CORS_ALLOWED_ORIGINS = [
    'https://graphiax.azurewebsites.net', # In our case
    'http://localhost:3000'  # If you are testing in a local host
]
```

## Some functions explanation
### get_network_structure()

The ```get_network_structure()``` function is responsible for converting the graph structure to JSON format, which contains both nodes and edges.

<img src="https://github.com/MohyiddineDilmi/GraphiaX/assets/33746487/9c3438be-5df2-44aa-8cb1-578f8ec37ecb" width="70%"/>

#
<img src="https://github.com/MohyiddineDilmi/GraphiaX/assets/33746487/cbbc29b6-a0a4-48a0-8454-ef657ef7f203" width="100"/>


