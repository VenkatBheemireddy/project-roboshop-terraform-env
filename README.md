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
4. At last, to destroy the infra you have to run as below:
    * make dev-destroy
    * make tst-destroy
    * make prd-destroy

NOTES:
1. If you don't see categories on the project home page then re-run "catalogue" component (i.e., make dev-apply app_name=catalogue).
2. In the worst case, delete and re-create the catalogue VM and then run make file again.


