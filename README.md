# Kubernetes Database Reader (Nagp)

These Kubernetes yamls sets up the infrastructe for a application to reads data from a MySQL database and provides it through a web service.

## Repository and Links

- **Repository URL:** [GitHub Repository](https://github.com/iyogita/kubernetesDatabaseReaderNagp)
- **Docker Hub URL:** [Docker Hub Repository](https://hub.docker.com/repository/docker/iyogita/demo-app/general)
- **Docker Image URL:** [Docker Image](https://hub.docker.com/layers/iyogita/demo-app/3.0/images/sha256-7664c768de0cdbc1f27d4efb30e44b288a0d3761840a8818449e94327803cce6?context=repo) (These are related java pplication images)
- **Service URL:** [http://35.239.191.156/records](http://35.239.191.156/records) (Note: External IP may change as cluster deletion is needed to avoid billing issues)
- **Recording URL:** [Presentation Video](https://nagarro-my.sharepoint.com/:v:/p/yogita_singh/ER4C6iQys-9Gifiu8HzFdxwBY8uPUwuXykuaw1g-jrh2gg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=HrAhFs)

## Description

The Kubernetes Database Reader (Nagp) is a yaml-based application designedset up infrastructe for a application to read data from a MySQL database. The data is exposed through a RESTful web service, making it accessible via HTTP requests.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Java Development Kit (JDK)
- Docker
- Kubernetes (kubectl)

### Installation

1. **Run Below Commands to setup the Infra:**

- kubectl apply -f dbsetup.yaml
- kubectl apply -f apisetup.yaml
- kubectl apply -f hpa.yaml

