#PowerAutomate #PowerAutomateCloud #Dataverse

# Power Automate Monitoring

A simple custom entity to wrap your automation solution elements in one place - made for organizations where **1** cloud flow connects to **1** desktop flow and runs on **1** specific machine (machine can be reused by other flows).

With this tool, you can build your custom oversight dashboards spanning all components required by your solution, and adding business context such as:
* automation name
* business department/function
* owner or team of owners

## How does it work?
Here's a list of your automations. Icons indicate last process outcome and whether a machine is connected to Power Automate 
![list of automation records, shows 1 process completed OK but it's machine is not connected now](screen1.png)

And here you can see the details of the process:
![screen of main form, showing links to cloud flow, desktop flow, machine](screen2.png)

## What are the built-in features?
* adding a cloud flow link (or updating it) will automatically link your automation record to the 1st desktop flow called from it, and will update the connection reference name
* adding a machine link will retrieve it's status (connected/offline) and software version
* flipping the "Update machine status" switch will update the connected/offline state (your switch will return to off when it's done, make sure you refresh the screen to see new data)
* also, all machines are queried for their status every 30 minutes

## Notes
There are no security roles provided, but you're welcome to extend this solution with a dedicated security role. You might consider creating a read-only role and one where people would only be able to see or modify their own automations.
