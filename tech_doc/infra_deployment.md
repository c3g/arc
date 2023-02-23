# Deployment Doc

The arc infrastructure deployment on the cloud uses Terraform + Ansible. Repo of each services can be found on the [C3G Github page](https://github.com/orgs/c3g) with the Terraform-<service name> and Ansibe-<service name> naming convention. Changes and updates are automatically pushed from github with actions when changes are made to the main and dev branches./

The core arc infrastructure documentation for internal consumption is [found on the c3g google drive](https://drive.google.com/drive/u/2/folders/1qVOhXMh39uR2EEpk8qw79sf5RU86jkWz)


We also try to get secondary services from the C3G Data and Techdev groups to be deployed with Podman in automated fashion. The two main services are 

* [bento](https://github.com/bento-platform/)
* [Project Tracking](https://github.com/c3g/project_tracking)

We also deploy the (magic castle project)[https://github.com/ComputeCanada/magic_castle] for data analysis purpose. We aim at integrating that project with or identification platform so user name and password can be detached from each deployments of the project.   