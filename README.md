
<img width="900" height="813" alt="Assignment-3-Test-SS" src="https://github.com/user-attachments/assets/bb6dddac-1620-49d6-98da-cfaeb01c8d3f" />
<img width="916" height="640" alt="Assignment3-SS-B-T-D" src="https://github.com/user-attachments/assets/8f9b0789-5983-4b72-a368-544acfadd926" />
<img width="936" height="373" alt="Assignment3-SS Pretty Print" src="https://github.com/user-attachments/assets/94d8c827-2db6-4ea3-8c74-212482926981" />
<img width="902" height="826" alt="Assignment-3-DeploySS" src="https://github.com/user-attachments/assets/287e1553-7a11-4a08-871c-daeaf0d3fb23" />
<img width="901" height="821" alt="Assignment3-Build SS" src="https://github.com/user-attachments/assets/91363f0a-9a16-4c18-977b-9170f512e9cd" />

\# GitHub Actions CI/CD Assignment



\## Objective

Demonstrate Continuous Integration and Continuous Deployment using GitHub Actions and Render.



\## Application

A Flask web application with two endpoints:

\- `/` — Returns a welcome message and success status.

\- `/health` — Returns the application's health status.



\## Technologies

\- Python 3.12

\- Flask

\- pytest

\- Gunicorn

\- GitHub Actions

\- Render



\## Workflow

Workflow file: `.github/workflows/ci-cd.yml`



The workflow runs on every push to the `main` branch.



\### Build

Installs dependencies and verifies that the application imports successfully.



\### Test

Runs unit tests using pytest for the home and health endpoints.



\### Deploy

Triggers deployment to Render after Build and Test pass. The deploy hook is stored securely in the GitHub repository secret `RENDER\_DEPLOY\_HOOK\_URL`.



\## Run Locally

Install dependencies:



```bash

pip install -r requirements.txt

```



Run tests:



```bash

python -m pytest -v

```



Start the app:



```bash

gunicorn app:app

```



\## Deployment

Live application: https://github-actions-assignment-m2ir.onrender.com



Health endpoint: https://github-actions-assignment-m2ir.onrender.com/health



\## Workflow Results

The latest workflow completed successfully with Build, Test, and Deploy passing.



\### Screenshots

Save your screenshots in the `screenshots` folder and use these filenames:

\- `build.png`

\- `test.png`

\- `deploy.png`

\- `workflow-success.png`



!\[Successful workflow](screenshots/workflow-success.png)



\## GitHub Repository

https://github.com/Shaheer8043/github-actions-assignment


