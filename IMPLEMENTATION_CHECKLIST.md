# Implementation Checklist

Build the application yourself using `PROJECT_BRIEF.md`.

## Initial setup

- [ ] Read the project specification.
- [ ] Review the architecture and data model.
- [ ] Create a Python virtual environment.
- [ ] Install and pin the required dependencies.
- [ ] Configure credentials through environment variables.
- [ ] Review the data privacy and security requirements.

## Project acceptance criteria

- [ ] POST /predict returns 200 with prediction ID
- [ ] SHAP vector persisted in DB
- [ ] Response time <200 ms for models <1 M parameters
- [ ] Runs as scheduled Docker container
- [ ] Generates an alert when distance >0.1
- [ ] Stores drift metrics in DB
- [ ] Dashboard updates within 5 min of new data
- [ ] Email sent with correct model & feature details
- [ ] Access control via simple token
- [ ] Initialize Git repo, Dockerfile, docker‑compose
- [ ] Configure PostgreSQL + pgvector schema
- [ ] Deploy MLflow server
- [ ] Implement /predict endpoint
- [ ] Integrate shap library with model loading from MLflow
- [ ] Persist predictions & SHAP vectors
- [ ] Create nightly drift job (Docker entrypoint)
- [ ] Implement Wasserstein distance calculation
- [ ] Configure email alert via SMTP
- [ ] Connect Grafana to PostgreSQL
- [ ] Build feature‑importance time series panels
- [ ] Write CI/CD workflow
- [ ] Unit tests for API validation (pytest)
- [ ] Integration tests for DB persistence
- [ ] Mock shap computation to test worker flow
- [ ] End‑to‑end test: submit prediction → verify SHAP stored → run drift job → verify alert
- [ ] Docker Compose for local development
- [ ] GitHub Actions builds multi‑arch image and pushes to Docker Hub
- [ ] Deploy to Render/ Railway (free tier) with PostgreSQL add‑on
- [ ] Configure environment variables for MLflow & SMTP

## Before completion

- [ ] Implement the planned MVP features.
- [ ] Add unit and integration tests.
- [ ] Run the test suite.
- [ ] Measure the evaluation metrics in the brief.
- [ ] Record actual results and known limitations.
- [ ] Document setup and deployment.
- [ ] Update the README to reflect the implemented features.
- [ ] Add only verified outcomes to your resume.
