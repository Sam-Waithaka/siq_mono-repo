# SIQ Mono-Repo

## Overview
This repository serves as the central hub for the SIQ project, incorporating three key components via Git submodules:

- **Frontend:** [SIQ Frontend](https://github.com/Sam-Waithaka/siq_frontend.git)
- **Backend:** [SIQ Backend](https://github.com/Sam-Waithaka/siq_backend.git)
- **Machine Learning & AI Integration:** [SIQ ML & AI Integration](https://github.com/Sam-Waithaka/siq_ml_and_ai_integration.git)

Each submodule contains its own detailed README with setup, usage, and deployment instructions.

## Mono-Repo Structure
To ensure modularity and maintainability, the project is structured using Git submodules within a mono-repo. This design allows each component (frontend, backend, and ML API) to be independently managed while remaining centrally organized. The advantages of this approach include:

- **Scalability:** Independent version control for each module
- **Modularity:** Components can evolve separately while maintaining integration
- **CI/CD Integration:** Simplified deployment pipeline across different services

## Key Implementations

### Backend (Django & DRF)
- RESTful API with JWT-based authentication
- User registration, login, and profile management
- PostgreSQL as the database
- API documentation with Swagger and Redoc

### Frontend (React.js)
- User authentication UI using React Hooks, React Router, and Axios
- Form validation with React Hook Form
- JWT authentication with local storage

### Machine Learning API (FastAPI & Scikit-Learn)
- Loan default prediction model
- Exposed as a REST API

## DevOps & Deployment
- The frontend and backend are separately dockerized
- Docker Compose for local development
- Kubernetes deployment on Azure (in progress, final push pending)
- CI/CD pipeline setup with GitHub Actions

## Getting Started
### Clone the Mono-Repo with Submodules
```bash
# Clone the mono-repo along with submodules
git clone --recurse-submodules https://github.com/Sam-Waithaka/siq_mono_repo.git
```

## Initialize Submodules (if already cloned without )

```bash
git submodule update --init --recursive
```

For further details, refer to each submodule’s README for specific setup and deployment instructions.