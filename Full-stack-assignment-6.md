# **Gift Shop Management Dashboard**

Each product must have the following information

- Product name
- Product price
- Product quantity

**Note: Additionally, ensure to include more product information based on the specified filter criteria mentioned in point 4.**

## **Requirements:**

**Objective:**
The primary objective of this assignment is to design and implement a comprehensive Gift Shop Management Dashboard, providing the tools to efficiently manage the gift inventory, track sales, and analyze sales history. The assignment will incorporate features such as authentication, CRUD operations, state management, real-time UI updates, gift filtering, user-based management with multiple roles, coupon & discount functionality, and invoice print options.

**Authentication:**

1. **User Registration and Login:**
    - Users must register and log in to access the dashboard.
    - Use JWT (JSON Web Tokens) for secure authentication.
    - Roles: Two roles - Manager and Seller.
        - Manager: Can add, delete, and modify products.
        - Seller: Can only sell products.

**Functionality:**

1. **Gift Shop Management:**
    - CRUD Operations:
        - Add a new gift to the inventory. (Manager only)
        - Delete existing gifts from the inventory. (Manager only)
        - Update gift details. (Manager only)
        - Read and view the list of gifts in the inventory.
        - Implement a robust filtering system to effectively narrow down gift selections based on various criteria.
2. **Sales Management:**
    - Users can search for a product to sell, and upon finding it, they can click the "Sell" button. On clicking the sell button, a form will pop up. The form will have the following fields:
        - Quantity of the product to be sold (Input quantity cannot exceed the current available stock of the product)
        - Name of the buyer
        - Date of the sale
        - Seller (auto-assigned based on the logged-in user - Seller role)
    
    **Note: If the quantity reaches zero, the product will be removed from the inventory.**
    
3. **Sales History:**
    - View sales history categorized by:
        - Weekly
        - Daily
        - Monthly
        - Yearly
4. **Gift Filtering (Implement on the gift management page)**
- Implement a comprehensive gift filter system to optimize inventory management. The filter options should cater specifically to gifts and novelty items:
    - **Filter by Price:** Allow users to set a price range for gifts.
    - **Filter by Occasion:** Provide options for filtering gifts based on occasions (e.g., birthdays, anniversaries, holidays).
    - **Filter by Recipient:** Implement a real-time search functionality for gift recipients to quickly find gifts for a specific person.
    - **Filter by Category:** Categorize gifts into categories (e.g., home decor, gadgets, accessories) and allow users to filter by their preferred categories.
    - **Filter by Theme:** Include a filter for gift themes to easily manage gifts with specific themes (e.g., vintage, modern, romantic).
    - **Filter by Brand:** Allow users to filter gifts based on brands.
    - **Additional Relevant Filter Parameters:** Introduce other relevant filter parameters such as material, color, or any custom attributes associated with the gifts.
1. **User Interface Features:**
    - Gracefully update the UI in real-time when changes occur (e.g., product updates, sales, etc.).
    - Utilize RTK Query for efficient CRUD operations.
    - Implement **Re-fetching** functionality to ensure data accuracy and consistency.
2. **State Management:**
    - Utilize Redux for state management to maintain a consistent application state.
3. **Bulk Delete Product Options:**
    - Enable users to efficiently manage their inventory by implementing a bulk delete feature for the gifts.
    - Provide a user-friendly interface to select and delete multiple gift options simultaneously.
4. **Duplicate & Edit Feature:**
    - Implement a feature within the product list that includes a button. Upon clicking this button, users will be redirected to a form where product data is pre-filled. Users can then make modifications as needed to create a new product based on the existing one. The button could be named "Duplicate & Edit" or "Create Variant" to convey the idea that users can duplicate an existing product and make modifications to create a new one.
5. **Coupon & Discount Functionality:**
    - Allow customers to provide a coupon code during checkout.
    - Sellers can input the coupon code, and customers receive a discount based on the coupon.
    - Managers can create a coupon code and store it in the database.
    - An API call can be implemented to verify the coupon and reduce the amount based on the coupon.
    - Don't forget to provide the coupon code when submitting the assignment for the examiner to check.
6. **Invoice download (PDF)**
        - After completing a sale, sellers will have the option to download the invoice for the order.
        - The invoice will contain details such as the product name, quantity, date, and name of the buyer.
        - Sellers can download the invoice for their records or for further processing.
        - For generating PDF invoices in a React application, you can use the following React PDF libraries:
            - **react-pdf**:
            - jspdf
            - react-pdf/renderer
            - react-to-print
7. **Additional Features:**
    - Implement any other relevant features that enhance the usability and functionality of the dashboard.

**Technical Requirements:**

- Use RTK Query for efficient CRUD operations.
- Implement Redux for state management.
- Ensure the UI updates gracefully in real-time.
- Use the **Re-fetching** functionality for data accuracy.
- Apply tags for improved organization and categorization.
- Optimize for mobile responsiveness to ensure a reasonable user experience on various devices.
- Ensure there are at least 10 commits in your GitHub repository.
- Avoid the use of AI tools or libraries for generating code. Write the code manually to demonstrate a clear understanding of the concepts.
- You can create the backend for this assignment on a single page, but we highly recommend applying the modular pattern we introduced in Level 2 for enhanced code organization and maintainability.

**Submission Guidelines:**

- Submit a well-documented codebase with clear comments.
- Make sure to add a README file that explains how to set up and use the application. In the README, include details like the project name, live URL, features, technology used, and other important information. Try to make it look professional by doing some research and making it appealing.

### **Submission:**

- Provide the GitHub repository links for the front-end and back-end, and ensure there is a README file with explicit instructions for running the application locally.
- Live deployment link
- Submit a demo video showcasing the functionality of the Inventory Management Dashboard.

**Note:**
The assignment should reflect best practices regarding code organization, security, and user experience. It should demonstrate proficiency in using the specified technologies and effectively address shopkeepers' needs to manage their inventory.

### **Deadline:**

- 60 marks: February 17, 2024 11.59 PM
- 50 marks: February 18, 2024 11.59 PM
- 30 marks: After February 18, 2024 11.59 PM
