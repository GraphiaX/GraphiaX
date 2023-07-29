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

<img src="https://github.com/MohyiddineDilmi/GraphiaX/assets/33746487/9329de75-42f3-4915-b003-5b863c56b112" width="70%"/>

# Frontend

Repo Link: https://github.com/MohyiddineDilmi/graphiax-frontend

GraphiaX Frontend Docker image: 
https://hub.docker.com/repository/docker/dilmi0000/graphiax-frontend/general

```JS
const BASE_URL = 'Your Server URL';
const url = `${BASE_URL}/react_api/info/`;
```

>💡 We will focus more on the backend.

# Backend

Repo Link: https://github.com/MohyiddineDilmi/graphiax-server

Requirments

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

<img src="https://github.com/MohyiddineDilmi/GraphiaX/assets/33746487/4d4e3b46-d3b4-425d-9d5d-52e2ac6f3ee3" width="70%"/>

## get_network_structure()

The ```get_network_structure()``` function is responsible for converting the graph structure to JSON format, which contains both nodes and edges.

<img src="https://github.com/MohyiddineDilmi/GraphiaX/assets/33746487/9c3438be-5df2-44aa-8cb1-578f8ec37ecb" width="70%"/>

