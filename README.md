# How to Create Junction Object in Salesforce

### What is a junction object?

A junction object in Salesforce is a custom object that is used to create a many-to-many relationship between two objects. This is achieved by using two master-detail relationships from the junction object to the two related objects.

### Steps to create Junction object

#### Step 1: Define the Objects Involved

Ensure that you have two objects that you want to relate to each other. These can be either standard or custom objects.

#### Step 2: Create the Junction Object

1. **Go to Setup**: Click the gear icon in the upper right and select "Setup".
2. **Navigate to Object Manager**: In the Setup menu, type "Object Manager" in the Quick Find box and select it.
3. **Create a New Custom Object**:
   * Click on "Create" and select "Custom Object".
   * Fill in the label and plural label for the junction object. For example, if you're relating "Projects" and "Employees", you might name it "Project Assignment".
   * Optionally, set the Record Name, Data Type, and other properties.
   * Click "Save".

#### Step 3: Create Master-Detail Relationships

1. **Add the First Master-Detail Relationship**:
   * In the junction object (e.g., "Project Assignment"), go to the "Fields & Relationships" section.
   * Click "New" and select "Master-Detail Relationship".
   * Choose the first related object (e.g., "Projects").
   * Follow the prompts to complete the setup and save.
2. **Add the Second Master-Detail Relationship**:
   * Still, in the junction object, go back to "Fields & Relationships".
   * Click "New" again and select "Master-Detail Relationship".
   * Choose the second related object (e.g., "Employees").
   * Follow the prompts to complete the setup and save.

#### Step 4: Configure Page Layouts and Related Lists

1. **Modify the Page Layouts for the Related Objects**:
   * In the Object Manager, go to each of the two related objects (e.g., "Projects" and "Employees").
   * Select "Page Layouts".
   * Edit the relevant page layout and add the junction object-related list (e.g., "Project Assignments").
   * Save the changes.
2. **Modify the Page Layout for the Junction Object**:
   * In the junction object, go to "Page Layouts".
   * Edit the layout to ensure it includes relevant fields and related lists.
   * Save the changes.

#### Step 5: Verify the Setup

1. **Test the Relationships**:
   * Create records in each of the two related objects (e.g., create a Project and an Employee).
   * In the related list for the junction object, add a new record and verify that you can relate the two objects through the junction object.

Refer to learn more  [Junction Objects in Salesforce](https://arrify.com/junction-object-in-salesforce/#Creating\_Records\_for\_Junction\_Object)&#x20;
