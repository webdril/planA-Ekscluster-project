This is a devops project that requires the deplyment of a kubernetes cluster from AWS through the use of terraform.

# Please go through the documentation below to create an EKS cluster from the codes in this repository.<br><br>

**Step 1:** Create a folder on your pc/mac desktop and name the folder projects.

**Step 2:** Open the projects folder from your file explorer, and once inside the folder, right click on an empty space and choose "open in terminal" from the list of options presented to you.


**Step 3:** While in the command prompt, type the following without the quotations "git clone https://github.com/webdril/planA-Ekscluster-project.git"<br>
The command above will clone the terraform repository into a folder named planA-Ekscluster-project.<br>
This folder was created automatically by the git clone https://github.com/webdril/planA-Ekscluster-project.git command, and it is created inside your projects folder that was created in step 1 above.

**Step 4:** Open the newly created folder called planA-Ekscluster-project, and once inside the folder, right click on an empty space and choose "open in terminal" from the list of options presented to you.

**Step 5:** Once in the terminal window also known as cli, type terraform init

**Step 6:** Then type terraform plan to be sure everything is working well.

**Step 7:** Then type terraform apply, and once a question is asked in the cli type yes to proceed with the deployment of the infrastructure

**Step 8:** Once the deployment is completed, the next thing to do is to install kubectl in to your work machine (windows pc to be precise). The following guide will help you achieve this https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/#install-on-windows-using-chocolatey-or-scoop

**Step 9:** To deploy/pull the images from docker hub, run the following command without the quotation "kubectl apply manifest.yml"

**Step 10:** After deployment, the next thing is to access the web app on your local browser. To do this, type the following command without the quotation "kubectl port-forward svc/microservice -n default 8080:3000"

**Step 11:** You can now access the app by typing the following in you browser without the quotation "http://127.0.0.1:8080