
_Prior to starting the **Exercise 8.1** in this chapter, you need to create a Security Group that will be used by your EC2 Instances which will act as your web/app servers for the solution we are trying to build over the upcoming chapters. We will call this Security Group,_ **'AppServers-SG'**. 

**Please follow these steps before starting Excercise 8.1:**

* Log into your AWS Management Console as the IAM user Alice you created in Chapter 4 and navigate to the VPC Dashboard [Ensure that you are in the same region where you have built your VPC so far (which should be the US-East-1 region).]

* Next, from the left-hand menu, select Security groups under the Security sub-heading

* In the right-hand pane, click the Create security group button

* For the Security group name, type in **AppServers-SG**

* In the description box type in "Allow RDP traffic from Bastion Hosts" for now.

* Under VPC, ensure you select ProductionVPC from the drop-down list.

* Next, in the Inbound roles section, click on the Add rule button

* Under Type, select RDP.

* Ensure that Source is set to Custom, and in the search box, start typing sg-. You should see that a list of all security groups shows up in a list. 

* Select the BastionHost-SG security group for now. We will later change this in upcoming exercises.

* Click on the Create security group button in the bottom right-hand corner of the screen.

_AWS will now confirm that the security group has been created successfully._
