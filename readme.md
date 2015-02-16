# IGSO mailing template for the IGSM 2015 meeting payment details
This is a fork of https://github.com/leemunroe/html-email-template

### The email template
The template was needed for creating formatted emails that were sent using an Excel VBA-based mailing script using private domain that was then connected to Zoho mail.
Each email was personalised with the person’s name and payment details. The side effect of using an email-to-email single address recipient list (vs. using Mailchimp and other mailer programs) was that it also reduces the chance of the mail being marked as spam. 

### Features
* Some layout improvements that were necessary for displaying the mail consistently across email clients.
* Placeholders in the form of %placeholder%, which can then be replaced programmatically.
* Visual buttons that are supported by Outlook by using conditional code.


### Issues (not necessary bugs, rather features)
Sadly the [Premailer](http://premailer.dialect.ca/), which is required for full email client compatibility has one issue with the template. It will break the  <![if !mso]> tags and will cause the Outlook client to show the buttons twice (once per Outlook code and then the general code that was supposed to be ignored).

### IGSO and Github
The IGSM event is an annual international student event hosted by a rotating new organising team. Transferring the information from one organiser to another has been traditionally done by zip files and the likes and gradually becoming wiki-based and now with a Github account.

This allows templates and files that are in the spirit of Github to be transferred from one year to the next without requiring passwords. This also allows to build upon the tools that have been created in the previous years, even if everything is not used at that particular event.
