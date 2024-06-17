# Controlling Field in Salesforce

### What is the Controlling Field in Salesforce?

In Salesforce, a controlling field controls how other fields on the same object or linked objects behave, are shown or are valued. It serves as a compass, affecting the data-entering procedure and guaranteeing accuracy and uniformity throughout your Salesforce organisation.

You can customise the user experience, uphold data integrity, and match your Salesforce instance to the particular procedures and needs of your company by making use of these fields.

### How do Controlling fields work?

1. **Identify Fields:**
   * Choose the controlling field and the dependent field.
2. **Establish Dependencies:**
   * Link the controlling field to the dependent field to define their relationship.
3. **Define Behavior:**
   * Specify how the dependent field reacts to each value of the controlling field, such as different picklist options.
4. **Dynamic Interaction:**
   * When users change the controlling field, Salesforce automatically updates the dependent field based on the set dependencies.

### Setting up controlling fields:

1. **Identify Fields:**
   * Choose a controlling field and a dependent field.
2. **Establish Relationship:**
   * Connect the dependent field to the controlling field.
3. **Define Behavior:**
   * Specify how the dependent field responds to different values of the controlling field.
4. **Test and Adjust:**
   * Ensure the setup works as intended, and make adjustments if needed.

### Use Case of Controlling fields:

Certainly, here are some straightforward use cases of controlling fields:

1. **Employee Onboarding Form:**
   * Controlling Field: Job Position
   * Dependent Field: Required Training
   * Based on the selected job position, the system shows the relevant training modules.
2. **Event Registration Form:**
   * Controlling Field: Event Type
   * Dependent Field: Ticket Options
   * Depending on the type of event selected, different ticket options (e.g., VIP, Standard) are presented.

**Refer to Learn More about** [**Controlling fields in Salesforce**](https://arrify.com/controlling-field-in-salesforce/#How\_Controlling\_Fields\_Works)
