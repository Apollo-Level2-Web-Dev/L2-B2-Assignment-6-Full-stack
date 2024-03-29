## Sports Items **Management Dashboard**

Each product must have following information

- Product name
- Product price
- Product quantity
- Product size
- Product branch

**Note: Additionally, ensure to include more product information based on the specified filter criteria mentioned in point 4.**

## **Requirements:**

**Objective:**
The primary objective of this assignment is to design and implement a comprehensive Sports Items Management Dashboard, providing the tools to efficiently manage the sports inventory, track sales, and analyze sales history. The assignment will incorporate features such as authentication, CRUD operations, state management, real-time UI updates, sports items filtering, and invoice download functionality.

**Authentication:**

1. **User Registration and Login:**
    - Users must register and log in to access the dashboard.
    - Use JWT (JSON Web Tokens) for secure authentication.
    - Two user roles: Super Admin, Branch Manager and Seller.
    - Super Admin will have all access, Managers can add and modify products, while Sellers can only sell.

**Functionality:**

1. Sports Items **Management:**
    - CRUD Operations:
        - Add a new sports item to the inventory.
        - Delete existing sports items from the inventory.
        - Update sports item details.
        - Read and view the list of sports items in the inventory.
        - Implement a robust filtering system to effectively narrow down sports item selections based on various criteria.
2. **Sales Management:**
    - Users can search for a product to sell, and upon finding it, they can click the "Sell" button. On clicking the sell button a form will pop up. The form will have the following fields:
        - Quantity of the product to be sold (Input quantity cannot exceed the current available stock of the product)
        - Branch (the branch of the seller will be automatically selected which cannot be changed)
        - Name of the buyer
        - Date of the sale
    - Invoice download (PDF)
        - After completing a sale, users will have the option to download the invoice for the order.
        - The invoice will contain details such as the product name, quantity, date, and name of the buyer.
        - Users can download the invoice for their records or for further processing.
        - For generating PDF invoices in a React application, you can use the following React PDF libraries:
            - **react-pdf**:
            - jspdf
            - react-pdf/renderer
            - react-to-print
        
    
    **Note: If the quantity reaches zero, the product will be removed from the inventory.**
    
3. **Sales History:**
    - View sales history categorized by :
        - Weekly
        - Daily
        - Monthly
        - Yearly
    - Super Admin can view All branch history either specific or any branch history. The branch manager only views his branch all history.
    - Super Admin and Branch Manager Download pdf Sales report on any date or all-time sales history. The sales report compares expenses and sales as per date to get a total amount that indicates profit or loss.
        
        
4. **Sports Items Filtering (Implement on the sports items management page)**
- Implement a comprehensive sports items filter system to optimize inventory management. The filter options should cater specifically to sports equipment and gear:
    - **Filter by Sport Type:** Allow users to set a filter for specific sports types (e.g., soccer, basketball, tennis).
    - **Filter by Brand:** Implement a real-time search functionality for sports item brands to quickly find items by a specific manufacturer.
    - **Filter by Size:** Enable searching by size for items like clothing and accessories.
    - **Filter by Price Range:** Allow users to set a price range for sports items.
    - **Filter by Material:** Include a filter for sports items based on their materials (e.g., leather, synthetic, fabric).
    - **Filter by Color:** Allow users to filter sports items based on colors.
    - **Filter by Condition:** Implement a filter for new or used items.
    - **Additional Relevant Filter Parameters:** Introduce other relevant filter parameters such as weight, style, or any custom attributes associated with the sports items.
1. **User Interface Features:**
    - Gracefully update the UI in real-time when changes occur (e.g., product updates, sales, etc.).
    - Utilize RTK Query for efficient CRUD operations.
    - Implement **Re-fetching** functionality to ensure data accuracy and consistency.
2. **State Management:**
    - Utilize Redux for state management to maintain a consistent application state.
3. **Bulk Delete Product Options:**
    - Enable users to efficiently manage their inventory by implementing a bulk delete feature for the sports items.
    - Provide a user-friendly interface to select and delete multiple sports item options simultaneously.
4. Implement a feature within the product list that includes a button. Upon clicking this button, users will be redirected to a form where product data is pre-filled. Users can then make modifications as needed to create a new product based on the existing one. The button could be named "Duplicate & Edit" or "Create Variant" to convey the idea that users can duplicate an existing product and make modifications to create a new one.
5. **Additional Features:**
    - Implement any other relevant features that enhance the usability and functionality of the dashboard.

**Technical Requirements:**

- Use RTK Query for efficient CRUD operations.
- Implement Redux for state management.
- Ensure the UI updates gracefully in real time.
- Use the **Re-fetching** functionality for data accuracy.
- Apply tags for improved organization and categorization.
- Optimize for mobile responsiveness to ensure a reasonable user experience on various devices.
- Ensure there are at least 10 commits in your GitHub repository.
- Avoid the use of AI tools or libraries for generating code. Write the code manually to demonstrate a clear understanding of the concepts.
- You can create the backend for this assignment in a single page, but we highly recommend applying the modular pattern we introduced in Level 2 for enhanced code organization and maintainability.

**Submission Guidelines:**

- Submit a well-documented codebase with clear comments.
- Make sure to add a README file that explains how to set up and use the application. In the README, include details like the project name, live URL, features, technology used, and other important information. Try to make it look professional by doing some research and making it appealing.

### **Submission:**

- Provide the GitHub repository links of the front-end and back-end and ensure there is a README file with explicit instructions for running the application locally.
- Live deployment link
- Submit a demo video showcasing the functionality of the Inventory Management Dashboard.

**Note:**
The assignment should reflect best practices regarding code organization, security, and user experience. It should demonstrate proficiency in using the specified technologies and effectively address shopkeepers' needs to manage their inventory.

### **Deadline:**

- 60 marks: February 17, 2024 11.59 PM
- 50 marks: February 18, 2024 11.59 PM
- 30 marks: After February 18, 2024 11.59 PM
