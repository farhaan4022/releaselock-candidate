# ReleaseLock Candidate

Candidate packaging repository for the ReleaseLock project.

This repository is intentionally untrusted from the perspective of the
ReleaseLock approval and deployment boundary.

Its responsibilities are limited to:

- pinning the selected upstream InvenTree release
- minimal container/configuration adaptations
- building candidate images
- publishing candidate images to the designated ECR repositories

This repository must not have permission to:

- approve releases
- sign release manifests
- update ECS services directly
- modify IAM
- use iam:PassRole
- modify the ReleaseLock gate
- write approved release evidence
