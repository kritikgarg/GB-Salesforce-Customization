# How to Generate PDF in Salesforce

### Steps to Create PDF in Salesforce:

Visualforce pages in Salesforce can be used to generate a PDF. The option to render pages as PDF documents is something that Visualforce offers, and it can be helpful for creating reports, invoices, or any other type of document that requires a set style.

#### Step 1: Create a Visualforce Page

1. **Go to Setup**: Click the gear icon in the upper right corner and select "Setup".
2. **Navigate to Visualforce Pages**: In the Quick Find box on the left side, type "Visualforce Pages" and select it.
3. **Create a New Page**: Click the "New" button to create a new Visualforce page.
4. **Enter Page Details**:
   * **Label**: Enter a name for the page (e.g., "InvoicePDF").
   * **Name**: This will auto-fill based on the label.
   * **Description**: Optionally, add a description.
   * **Markup**: Enter the Visualforce markup for your page. Below is an example of a simple Visualforce page that generates a PDF for an invoice.

```html
<apex:page renderAs="pdf" controller="InvoiceController">
    <h1>Invoice</h1>
    <p>Invoice Number: {!invoice.Number}</p>
    <p>Date: {!invoice.Date}</p>
    <p>Customer: {!invoice.CustomerName}</p>
    <p>Total Amount: {!invoice.TotalAmount}</p>
</apex:page>
```

5. **Save the Page**: Click the "Save" button.

#### Step 2: Create an Apex Controller (if needed)

If you need to pull data from Salesforce objects, you’ll need an Apex controller to handle the data retrieval. Here’s an example controller that fetches invoice details:

1. **Navigate to Apex Classes**: In the Quick Find box, type "Apex Classes" and select it.
2. **Create a New Class**: Click the "New" button to create a new Apex class.
3. **Enter Class Details**:
   * **Class Name**: Enter a name for the class (e.g., "InvoiceController").
   * **Class Body**: Enter the Apex code for your controller. Below is an example of a simple controller.

```apex
public class InvoiceController {
    public Invoice__c invoice { get; private set; }

    public InvoiceController() {
        // Replace 'someInvoiceId' with the actual invoice ID or pass it as a parameter
        String invoiceId = ApexPages.currentPage().getParameters().get('id');
        invoice = [SELECT Id, Number__c, Date__c, CustomerName__c, TotalAmount__c FROM Invoice__c WHERE Id = :invoiceId];
    }
}
```

4. **Save the Class**: Click the "Save" button.

#### Step 3: Link Visualforce Page and Controller

1. **Edit the Visualforce Page**: Go back to your Visualforce page.
2. **Specify the Controller**: Add the controller to the page.

```html
<apex:page renderAs="pdf" controller="InvoiceController">
    <h1>Invoice</h1>
    <p>Invoice Number: {!invoice.Number__c}</p>
    <p>Date: {!invoice.Date__c}</p>
    <p>Customer: {!invoice.CustomerName__c}</p>
    <p>Total Amount: {!invoice.TotalAmount__c}</p>
</apex:page>
```

3. **Save the Page**: Click the "Save" button.

#### Step 4: Generate the PDF

To generate the PDF, you need to access the Visualforce page with the required parameters. For example:

1. **Access the Page**: Open the Visualforce page URL in your browser, passing the necessary parameters (e.g., invoice ID).

```
https://yourInstance.salesforce.com/apex/InvoicePDF?id=someInvoiceId
```

2. **View the PDF**: The Visualforce page should be rendered as a PDF document.

#### Additional Tips

* **Styling the PDF**: You can use CSS within the Visualforce page to style the PDF document.
* **Complex Documents**: For more complex documents, you can include tables, images, and other HTML elements in the Visualforce markup.
* **Testing**: Ensure you test the PDF generation with various data sets to ensure the layout and content are correctly rendered.

Refer to learn more [Generate PDF in Salesforce](https://arrify.com/generate-pdf-in-salesforce/)
