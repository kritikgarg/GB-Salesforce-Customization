# Email Action Salesforce

### What is an Email Action in Salesforce?

It aims at enabling users working on Salesforce to send emails directly within the Salesforce environment, through the use of Email Action. If performed using this function, it means the emails being provided respond automatically to chosen conditions, such as the occurrence of an event, or compliance with a set standard or workflow, hence the effectiveness of the messages given at every given time, with no need for daily monitoring.

### Implementing Email Action

1. **Create Email Templates**: Start by designing your email templates in Salesforce. Use merge fields to pull in dynamic data from your Salesforce records.
2. **Set Up Email Alerts**: Navigate to the Workflow Rules and create a new rule. Define the criteria that will trigger the email alert.
3. **Configure the Email Action**: In the Workflow Rule, add a new Email Alert action. Select the email template you created and specify the recipients.
4. **Activate the Workflow Rule**: Once everything is set up, activate the workflow rule to start automating your emails.

### Email Action Parameter in Salesforce

1. **Email Template**:
   * **Purpose**: Defines the content and format of the email.
2. **Recipient Type**:
   * **Purpose**: Specifies who will receive the email.
3. **Recipient email addresses**:
   * **Purpose**: Lists the actual email addresses to which the email will be sent.
4. **Related record ID**:
   * **Purpose**: associate the email with a specific Salesforce record.
5. **Sender Email Address**:
   * **Purpose**: Determines the 'From' address for the email.
6. **CC and BCC**:
   * **Purpose**: Allows you to send copies of the email to additional recipients.
7. **Email Encoding**:
   * **Purpose**: Sets the character encoding for the email content.
8. **Email Attachments**:
   * **Purpose**: Allows you to include files with the email.

Refer to learn more [Email Action](https://arrify.com/email-action-salesforce/).\
