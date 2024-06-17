# How to Create User in Salesforce

### What is a User in Salesforce?

In Salesforce, a "user" is a person who has been given access to the system by the organisation to do data entry, reporting and customer relationship management. They are identified by their login and password.

### Steps to Create a User in Salesforce

Creating a user in Salesforce involves several steps. Here's a step-by-step guide to help you create a new user:

#### Step 1: Log in to Salesforce

* Log in to your Salesforce instance with an account that has the necessary permissions to create users (typically a System Administrator).

#### Step 2: Navigate to User Management

1. **Go to Setup**: Click the gear icon in the upper right corner and select "Setup".
2. **Find Users**: In the Quick Find box on the left side, type "Users" and select "Users" under the "Users" section.

#### Step 3: Create a New User

1. **Click New User**: On the Users page, click the "New User" button.
2. **Fill in User Details**:
   * **First Name**: Enter the first name of the user.
   * **Last Name**: Enter the last name of the user.
   * **Alias**: This is typically auto-filled but can be customized.
   * **Email**: Enter the user’s email address.
   * **Username**: Enter a unique username in the format of an email address (does not need to be a valid email).
   * **Nickname**: This is auto-filled but can be customized.
   * **Title**: Enter the user’s job title.
   * **Company**: Enter the company name.
   * **Department**: Enter the department name.
   * **Division**: Enter the division name.
   * **Role**: Select the role for the user from the dropdown menu.
   * **User License**: Select the appropriate user license (e.g., Salesforce, Salesforce Platform).
   * **Profile**: Select the appropriate profile which defines the user's permissions.
   * **Locale Settings**: Set the locale, language, time zone, and other settings as needed.
   * **Mailing Address**: Enter the user’s mailing address.
   * **Phone**: Enter the user’s phone number.
   * **Mobile**: Enter the user’s mobile number.
   * **Fax**: Enter the user’s fax number.

#### Step 4: Assign User Permissions and Settings

1. Feature Licences: If more feature licences are required, assign them (e.g., Marketing User, Knowledge User).&#x20;
2. Profile Settings: Verify that the chosen profile has the appropriate rights for the tasks the user needs to perform under the profile settings.

#### Step 5: Save and Notify User

* **Save**: Click the "Save" button to create the user. Salesforce will send an email to the new user with login instructions.

#### Optional Steps

* **Clone User**: If you need to create multiple users with similar settings, you can use the "Clone" feature on an existing user to quickly duplicate the setup.
* **Deactivate or Freeze User**: If needed, you can deactivate or freeze a user account from the Users page by clicking the "Deactivate" or "Freeze" link next to the user's name.

#### Additional Tips

* **Profile Customization**: Ensure the user's assigned profile has the correct permissions and settings.
* **Role Hierarchy**: Make sure the role hierarchy is set up correctly to align with your organization’s structure.

Refer to learn more about [Creating a User in Salesforce](https://arrify.com/create-a-user-in-salesforce/)
