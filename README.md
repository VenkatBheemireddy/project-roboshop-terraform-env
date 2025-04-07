**Terraform Roboshop Project with multi environment
(project-roboshop-terraform-env)**

**Databases:** mongodb, mysql, rabbitmq, redis

**Servers:** catalogue, user, cart, shipping, payment

**UI (ProxyServer):** frontend


**Project Running Steps:**
1. Run the Makefile as below to create all the VMs and their OS setup.
    * make dev-apply 
    * make tst-apply 
    * make prd-apply 
2. After completion of the above step, open the browser and run (http://<public-ip-address>).
3. You will get the roboshop home page.

NOTES: To destroy the infra you have to run as below:
    * make dev-destroy
    * make tst-destroy
    * make prd-destroy



