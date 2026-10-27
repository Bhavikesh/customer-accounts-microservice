# Customer Accounts Microservice — Capstone Submission Deliverables Checklist

This document maps all 33 capstone assignment questions/tasks to their deliverables, verified filenames, URLs, and current verification status.

## Verification Status Legend
- **VERIFIED**: Deliverable generated, executed with genuine output, and verified on public GitHub or local disk.
- **BLOCKED**: Requires live browser capture on GitHub Projects board (to prevent fabricating fake screenshots) or access to an active OpenShift/Kubernetes cluster in the course lab environment.
- **NOT COMPLETED**: Task not yet started.

---

## 33 Assignment Questions Mapping

| # | Task Requirement | Deliverable / Path | Status | Verification Details |
|---|---|---|---|---|
| **1** | Public GitHub README.md URL | `README.md` | **VERIFIED** | [README.md](https://github.com/Bhavikesh/customer-accounts-microservice/blob/main/README.md) verified live with CI badge, architecture, endpoints table, testing and container guides. |
| **2** | Public GitHub user-story.md URL | `user-story.md` | **VERIFIED** | [user-story.md](https://github.com/Bhavikesh/customer-accounts-microservice/blob/main/user-story.md) verified live in repository root and issue template. |
| **3** | planning-userstories-done.png | `submission-evidence/planning-userstories-done.png` | BLOCKED (Awaiting Screenshot) | Requires screenshot of GitHub Projects Kanban board with user stories #1 through #10 in the *New Issues* column. |
| **4** | planning-productbacklog-done.png | `submission-evidence/planning-productbacklog-done.png` | BLOCKED (Awaiting Screenshot) | Requires screenshot of GitHub Projects Kanban board with user stories moved to the *Ice Box* column. |
| **5** | planning-labels-done.png | `submission-evidence/planning-labels-done.png` | BLOCKED (Awaiting Screenshot) | Requires screenshot of GitHub Projects board with cards in *Product Backlog* showing `Technical Debt` and `enhancement` labels. |
| **6** | planning-kanban-done.png | `submission-evidence/planning-kanban-done.png` | BLOCKED (Awaiting Screenshot) | Requires screenshot of GitHub Projects board with Sprint 1 stories (#1 to #5) moved into the *Sprint Backlog* column with story estimates. |
| **7** | Public GitHub setup.cfg URL | `setup.cfg` | **VERIFIED** | [setup.cfg](https://github.com/Bhavikesh/customer-accounts-microservice/blob/main/setup.cfg) verified live; configured with nosetests (verbosity=2, spec, coverage), coverage reporting, flake8 exclusions, pylint. |
| **8** | rest-techdebt-done.png | `submission-evidence/rest-techdebt-done.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Setting up the development environment" (#1) card moved to *Done*. |
| **9** | read-accounts.png | `submission-evidence/read-accounts.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Read an account from the service" (#2) card moved to *Done*. |
| **10** | list-accounts.png | `submission-evidence/list-accounts.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "List all accounts in the service" (#3) card moved to *Done*. |
| **11** | update-accounts.png | `submission-evidence/update-accounts.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Update an account in the service" (#4) card moved to *Done*. |
| **12** | delete-accounts.png | `submission-evidence/delete-accounts.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Delete an account from the service" (#5) card moved to *Done*. |
| **13** | rest-create-done | `submission-evidence/rest-create-done` | **VERIFIED** | Live `curl -s -i -X POST` captured with HTTP 201 Created and `Location: https://127.0.0.1:8080/accounts/1`. |
| **14** | rest-list-done | `submission-evidence/rest-list-done` | **VERIFIED** | Live `curl -s -i` to `/accounts` captured with HTTP 200 OK and JSON array of created accounts. |
| **15** | rest-read-done | `submission-evidence/rest-read-done` | **VERIFIED** | Live `curl -s -i` to `/accounts/1` captured with HTTP 200 OK and account payload. |
| **16** | rest-update-done | `submission-evidence/rest-update-done` | **VERIFIED** | Live `curl -s -i -X PUT` to `/accounts/1` captured with HTTP 200 OK and updated payload. |
| **17** | rest-delete-done | `submission-evidence/rest-delete-done` | **VERIFIED** | Live `curl -s -i -X DELETE` to `/accounts/1` (HTTP 204 No Content) and subsequent GET (HTTP 404 Not Found). |
| **18** | sprint2-plan.png | `submission-evidence/sprint2-plan.png` | BLOCKED (Awaiting Screenshot) | Screenshot of board showing Sprint 2 user stories (#6 and #7) moved to *Sprint Backlog*. |
| **19** | ci-workflow-done | `submission-evidence/ci-workflow-done.txt` | **VERIFIED** | Genuine GitHub Actions workflow run log for Run ID 40519761913 saved; all jobs (setup, container initialization, flake8, pylint, nose with PostgreSQL) completed with status success. |
| **20** | ci-kanban-done.png | `submission-evidence/ci-kanban-done.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Need the ability to automate continuous integration checks" (#6) moved to *Done*. |
| **21** | Public GitHub ci-build.yaml URL | `.github/workflows/ci-build.yaml` | **VERIFIED** | [.github/workflows/ci-build.yaml](https://github.com/Bhavikesh/customer-accounts-microservice/blob/main/.github/workflows/ci-build.yaml) verified live on GitHub. |
| **22** | Public GitHub __init__.py URL | `service/__init__.py` | **VERIFIED** | [service/__init__.py](https://github.com/Bhavikesh/customer-accounts-microservice/blob/main/service/__init__.py) verified live; Flask application initialized with Talisman security headers and CORS. |
| **23** | security-headers-done | `submission-evidence/security-headers-done` | **VERIFIED** | Genuine `nosetests` output verifying Talisman security headers and CORS; 30 tests passed with 98% coverage. |
| **24** | security-kanban-done.png | `submission-evidence/security-kanban-done.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Need to add security headers and CORS policies" (#7) moved to *Done*. |
| **25** | sprint3-plan.png | `submission-evidence/sprint3-plan.png` | BLOCKED (Awaiting Screenshot) | Screenshot of board showing Sprint 3 user stories (#8, #9, #10) moved to *Sprint Backlog*. |
| **26** | kube-app-output | `submission-evidence/kube-app-output` | **VERIFIED** | Genuine JSON output `{"name":"Account REST API Service","paths":"http://127.0.0.1:8081/accounts","version":"1.0"}` captured from live running Docker container. |
| **27** | kube-docker-done.png | `submission-evidence/kube-docker-done.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Containerize your microservice using Docker" (#8) moved to *Done*. |
| **28** | kube-kubernetes-done.png | `submission-evidence/kube-kubernetes-done.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Deploy your Docker image to Kubernetes" (#9) moved to *Done*. |
| **29** | Public GitHub Dockerfile URL | `Dockerfile` | **VERIFIED** | [Dockerfile](https://github.com/Bhavikesh/customer-accounts-microservice/blob/main/Dockerfile) verified live on GitHub using `python:3.9-slim` and non-root user `theia`. |
| **30** | kube-images | `submission-evidence/kube-images` | **VERIFIED** | Genuine `docker images accounts:1.0` output capturing image tag, image ID (90509c4396e3), disk usage, and size. |
| **31** | kube-deploy-accounts | `submission-evidence/kube-deploy-accounts.txt` | BLOCKED (Requires Cluster) | Ready to capture via `kubectl get all -l app=accounts` once applied to course OpenShift/Kube cluster. |
| **32** | pipelinerun.txt | `submission-evidence/pipelinerun.txt` | BLOCKED (Requires Cluster) | Ready to capture via `tkn pipeline start cd-pipeline --showlog` in course lab environment. |
| **33** | cd-pipeline-done.png | `submission-evidence/cd-pipeline-done.png` | BLOCKED (Awaiting Screenshot) | Screenshot showing "Create a CD pipeline to automate deployment to Kubernetes" (#10) moved to *Done*. |
