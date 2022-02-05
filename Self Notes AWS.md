AWS Technology Steps needed to complete homework


Precurser:  (try and gather/add these notes as well at some point)
	
	Add AWS account (using less needed email, in case have to close)
	Add IAM user account, to be regular-access point (rather than main acct)
	Save IAM user login info (including URL) somewhere safe


Step 1:  Log in to AWS using IAM user account (and URL)

	Confirm that location (upper right corner, left of login id) is Oregon
			(diff locations have diff sw packages, Oregon package
			is the one most applicable to this class)

	Go to billing info 

		User ID
		Billing Dashboard

		And confirm there aren’t a bunch of charges getting run up

	Click on AWS in top left to get back to main screen

	Ready to get started!


Step 2:  

	Set up bucket for data storage
	To get links, check to left of particular icon when they're in place, and then above there is a list of options, and one of them is to 'copy url'. 

	(if using JL , or including images in work)  

Depending on utilization:

	If Jupyter Lab - set up notebook instance


	If lex – Set up new Bot

		Do process

		Download program pending completion


Notes on Lambda function code updates:

Each time you update the code, the ‘Changes not deployed’ box prompts you to click the ‘Deploy’ button. 

Then can click on the ‘Amazon Lex’ browser window, and rebuilt the bot itself.



Lambda function testing:

	In window for lambda function, midway down page, to the right of yellow “code’ selection is test, then monitor.. the monitor tab opens up to the cloudwatch monitor, which shows any errors in a copy-able presentation.

	Within Cloudwatch, the options are logs and traces,
		Underneath that is ‘view logs in CloudWatch’ 
		and then there is a list of 'log events' that are time stamped. 
		For the line with the actual error, click on the triangle on the left - 
		the detail window will open up with line numbers and more info.
		And the 'COPY' button over on the right lets you copy the error text to paste 
		 into Stack Overflow or wherever.
		Each time through, the most recent run will be on top.
		
	Each new Cloudwatch tab includes all activity, replacing prior tabs in functionality
	
	If switching among lambda files in the Lex window, be sure to switch in the lambda window before looking at the log! Otherwise just looking at log for a different program - not useful.


PS the cloudwatch tab remains, and can just be closed (after multiple iterations will be multiple tabs)

Back to Lex: do build (or re-do after lambda code change)
Test
After works, click ‘Publish’ and give it an alias name

Export as zipped file:
	Go back to main amazon lex page, that shows your bot in the bot list
	Click on radio button to left of bot name
	Click on Actions
	Click on Export
	Choices: Bot version (1), Platform (Amazon Lex vs Alexa Skills Kit –ASK)

	That will open the usual file-download window on your computer, can save
		(into downloads folder) and continue from there



Stopping for the day:

	Download program pending completion
 (if not already done)

	Terminate JL instance
	Terminate robo instance
	Terminate data bucket




	
