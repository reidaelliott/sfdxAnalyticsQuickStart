This is an example workspace to get users quickly started to see the power of SFDX to develop analytics templates.  This assumes you have SFDX installed already and have authenticated to a developer hub.  If not see the quick start guide for the CLI installer:  https://developer.salesforce.com/tools/sfdxcli 

Also, to install the Analytics SFDX plugin run:

sfdx plugins:install @salesforce/analytics

After cloning this repo and navigating to the sfdxAnalyticsQuickStart directory in a terminal:

1.  Update the adminEmail in config/project-scratch-def.json to your email address
2.  Authenticate to your dev hub
3.  Create a scratch org 'sfdx force:org:create -s -f config/project-scratch-def.json .  This will create an scratch org which is ready with Analytics enabled.
4.  Push the sample analytics template in this workspace by running 'sfdx force:source:push'

At this point you have a scratch org with an Analytics template installed.  Explore the analytics commands by running 'sfdx analytics --help'

To view the Analytics template:
'sfdx analytics:template:list'
To create an Analytics application from the template
'sfdx analytics:app:create -t <templateid>

