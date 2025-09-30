<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 Pro, version 22H2 - x64 Gen2

<h2>Ticket Lifecycle Stages</h2>

- Intake (Receive Ticket)
- Assignment and Communication (Assigning the Ticket Appropriately)
- Working the Issue (Work Through the Ticket Giving Updates to the Customer)
- Resolution (Close the Ticket)

<h2>In Depth Photo Guided Lifecycle Stages</h2>

<p>
<img width="697" height="206" alt="image" src="https://github.com/user-attachments/assets/a6ce258a-cec0-46cf-be7d-452f6901c4ab" />
</p>
<p>
Before we begin creating tickets for us to "solve" we are going to delete the maintenance department because when we start creating tickets they for some reason get defaulted to this even if we deactivate it, so we're just going to delete it. To do that go to the admin panel, then agents, and then departments so from there just check the box next to "maintenence" and on the right side you should see a "more" tab click the drop down menu and hit delete so we don't have to worry about it bothering the lab later on. Now that page if you remember we accessed from this (http://localhost/osTicket/scp/login.php) URL, we are now going to step out of the admin/agent site and go to our users site to create some tickets for us to "work" on. The URL if you don't have it, is (http://localhost/osTicket) and this will take you to where we create some tickets!
</p>
<br />

<p>
<img width="643" height="376" alt="image" src="https://github.com/user-attachments/assets/13ea3874-4438-4233-b7b8-7b7c83563fe3" />
</p>
<p>
Once we get to the new site we will go to the "Open a New Ticket" tab at the top, and use the credentials you should have saved from the previous lesson. From here you will enter your fake email address associated with the user account, my user is Karen, and after I enter her credentials I will choose the help topic she will base the ticket around. For the this ticket set the help topic to "report a problem" and put "Entire mobile/online banking system is down" under the 'issue Summary' now for the large text box just detail what is happening, like "Our customers and agents haven't been able to load the banking portal, and anyone who can load it their login creds don't work." that will give the agent (you) more information to go off of, you'll still likely have to call the customer and follow up with any additional detail they may be able to provide, after you put all the information in click "create ticket". Now we'll log back into the agent portal but this time as John (you should have the credentials saved somewhere), and find the ticket we just made. 
</p>
<br />

<p>
<img width="726" height="391" alt="image" src="https://github.com/user-attachments/assets/493edfea-5754-4120-9fcc-8e4284d91acf" />
</p>
<p>
The ticket we just made will be under the tickets tab and if it isn't, make sure you fully deleted the "maintenance" department so it will go to the support team where John can see it. Now click on the ticket to open it, from here we'll review the ticket and if this were a real person we'd give the user a call or shoot an email to clarify anything you're unsure of. Now that we have all the information as of right now, we will change the ticket to match the situation. On the ticket, start by clicking "SLA Plan" and change it to Sev-A, since this problem is so wide spread and it is affecting every banking customer this would be considered to have a serious impact on the business. Now we want to change the help topic, so we'll do that by clicking "Help Topic" and changing it to "Report a Problem/ Business Critical Outage", in your job you will do this a lot where the user input information that will need to be updated based on how you understand the problem and its severity. At the bottom of the ticket there will be a place where you can see a 'history' of changes made to the ticket and by who, as well as communicate directly to the user updating them on the progression of their problem. With every ticket we want to give an update pretty regularly, more frequent with larger problems but still on the ball with smaller problems, even if no progress has been made we want them to know we haven't forgotten about them and we are working on their issue.
</p>
<br />

<p>
<img width="710" height="222" alt="image" src="https://github.com/user-attachments/assets/294feb72-21eb-47d4-a143-ba31bfb94ebb" />
</p>
<p>
One of the last steps for this ticket is after updating all the information we'll assign the ticket to the appropriate teams, and since this is a banking issue we'll assign it to the online banking team (To ensure you see this as an option make sure you have agents assigned to these teams.(you can do so in the admin panel under agents and teams click on "Online Banking" and add agents to it). Sometimes when the person who receives the ticket isn't qualified to handle it they will assign it outside their team or even department (to the admins perhaps) and it will remove them from having access to modify the ticket afterwards. Once that happens the online banking team will resolve the ticket, but since it's just a lab we'll go through how to close the ticket on our own. So let's say we were able to resolve the ticket, now we'd go to status and click "Open" we would change it to "Resolved" and that would be our first ticket done. (Just as a side note, sometimes you might come across high profile people like CFOs, Executive Staff, etc. making tickets, and you'll think it's always a Sev-A because of their position but sometimes they aren't as important on a business impact scale, so its always important to remember business impact)
</p>
<br />

<p>
<img width="507" height="417" alt="image" src="https://github.com/user-attachments/assets/937b9173-7b7c-49d7-97d7-a289923a563c" />
</p>
<p>
I wanted to make this lab with just one OMNI-Ticket that shows you all the mechanics from creating a ticket, to communicating with someone about the ticket, then correcting the ticket itself and appropriately assigning it to the right team, to lastly closing/resolving a ticket. You can now mess around with what we just walked through together and make some new diverse tickets and practice closing them after you've corrected them. If you close a ticket you want to review afterwards login as an admin and they will show all past tickets closed or resolved as well as their history.
</p>
<br />

<p>
<img width="333" height="180" alt="image" src="https://github.com/user-attachments/assets/350f382d-9963-4225-ae27-20f97658288e" />
</p>
<p>
Now we have officially reached the end of the lab, if you wish to keep this VM's open to work on tickets then remember to stop them when you are not working on them in Azure, but if you do plan to delete the VM's I personally find it fast to go to the resource group that houses the VM and take the both out from there. Always double check everything is deleted before you walk away. These VM's can get expensive if left on for a long period of time. Thank all of those who chose to dedicate some time to my guides and I hope they were helpful as you progress your IT career!
</p>
<br />
