# netdevops-ansible-ee
NetDevOps Ansible Execution Environment

Build image with:

    pip install ansible-builder
    ansible-builder build --tag netdevops-ansible-ee --container-runtime docker

More Details about Execution Envoronments can be found here:
- https://www.ansible.com/blog/introduction-to-ansible-builder
- https://ansible-builder.readthedocs.io/en/latest/
- https://ansible-runner.readthedocs.io/en/latest/execution_environments.html

Using ansible-runner for testing requires the lastest version from GitHub. Current PyPi version 1.4.6 is not working.

    pip install git+https://github.com/ansible/ansible-runner.git
    ansible-runner playbook --container-image=netdevops-ansible-ee --container-runtime docker test.yml
