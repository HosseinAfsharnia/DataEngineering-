# Question 1

Here is the the command and its following results to answer this question:
```bash
hossein@hossein-virtual-machine:~/Documents/DataEngineering-/01_Containerization-and-IaC$ sudo docker run -it --entrypoint=bash python:3.12.8
Unable to find image 'python:3.12.8' locally
3.12.8: Pulling from library/python
fd0410a2d1ae: Pull complete 
bf571be90f05: Pull complete 
684a51896c82: Pull complete 
fbf93b646d6b: Pull complete 
12f3828c4288: Pull complete 
4d8be491b866: Pull complete 
ec162e081748: Pull complete 
Digest: sha256:2e726959b8df5cd9fd95a4cbd6dcd23d8a89e750e9c2c5dc077ba56365c6a925
Status: Downloaded newer image for python:3.12.8
root@25af461324b4:/# pip --version
pip 24.3.1 from /usr/local/lib/python3.12/site-packages/pip (python 3.12)
root@25af461324b4:/#
```


# Question2

The `docker-compose.yaml` file mentioned that the `pgAdmin` container needs to connect to the `db` (PostgreSQL) container. The hostname is the name of the `db` service in the `docker-compose.yaml` file, which is set to `postgres`.

Therefore the Hostname is `postgres` and the Port is `5432`

# Question3 - 6
Skipped for the time being


# Question7

The correct sequence that describes the workflow for:

##### 1.Downloading the provider plugins and setting up the backend:
 For this purpose `terraform init`usally does that by initializing the Terraform working directory and downloading the necessary provider plugins and backend configuration.

##### 2.Generating proposed changes and auto-executing the plan:
To do so `terraform apply -auto-approve` can be used. It automatically applies the changes without requiring user approval for the plan.

##### 3.Remove all resources managed by Terraform:
`terraform destroy`does this job for us. It destroys all the resources defined in the Terraform configuration.

Therefore the correct answer is: 
`terraform init`, `terraform apply -auto-approve`, `terraform destroy`
