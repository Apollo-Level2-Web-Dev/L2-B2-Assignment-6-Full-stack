## Flower Management Dashboard

Each product must have the following information

- Product name
- Product price
- Product quantity

**Note: Additionally, ensure to include more product information based on the specified filter criteria mentioned in point 4.**

## **Requirements:**

**Objective:**
The primary objective of this assignment is to design and implement a comprehensive Flower Management Dashboard, providing the tools to efficiently manage the flower inventory, track sales, analyze sales history, and introduce customer membership with point rewards on purchases. The assignment will incorporate features such as authentication, CRUD operations, state management, real-time UI updates, flower filtering, and customer membership with points.

**Authentication:**

1. **User Registration and Login:**
    - Users must register and log in to access the dashboard.
    - Use JWT (JSON Web Tokens) for secure authentication.
    - Roles: Two roles - Manager and Seller.
        - Manager: Can add and modify products.
        - Seller: Can only sell products.

**Functionality:**

1. Flower **Management:**
    - CRUD Operations:
        - Add a new flower to the inventory. (Manager only)
        - Delete existing flowers from the inventory. (Manager only)
        - Update flower details. (Manager only)
        - Read and view the list of flowers in the inventory.
        - Implement a robust filtering system to effectively narrow down flower selections based on various criteria.
2. **Sales Management:**
    - Sales Man can search for a product to sell, and upon finding it, they can click the "Sell" button. On clicking the sell button a form will pop up. The form will have the following fields:
        - Quantity of the product to be sold (Input quantity cannot exceed the current available stock of the product)
        - Name of the buyer
        - Date of the sale
        - Sales Man (auto-assigned based on the logged-in user - Sales Man role)
    
    **Note: If the quantity reaches zero, the product will be removed from the inventory.**
    
3. **Sales History:**
    - View sales history categorized by:
        - Weekly
        - Daily
        - Monthly
        - Yearly
4. **Flower Filtering (Implement on the flower management page)**
- Implement a comprehensive flower filter system to optimize inventory management. The filter options should cater specifically to flowers and floral arrangements:
    - **Filter by Price:** Allow Salesman to set a price range for flowers.
    - **Filter by Bloom Date:** Provide options for filtering flowers based on their bloom date.
    - **Filter by Color:** Implement a real-time search functionality for flower colors to quickly find flowers of a specific hue.
    - **Filter by Type:** Categorize flowers into types (e.g., roses, lilies, sunflowers) and allow Salesman to filter by their preferred categories.
    - **Filter by Size:** Include a filter for flower sizes to easily manage flowers of specific sizes.
    - **Filter by Fragrance:** Allow Salesman to filter flowers based on their fragrance.
    - **Additional Relevant Filter Parameters:** Introduce other relevant filter parameters such as arrangement style, occasion, or any custom attributes associated with the flowers.
1. **User Interface Features:**
    - Gracefully update the UI in real-time when changes occur (e.g., product updates, sales, etc.).
    - Utilize RTK Query for efficient CRUD operations.
    - Implement **Re-fetching** functionality to ensure data accuracy and consistency.
2. **State Management:**
    - Utilize Redux for state management to maintain a consistent application state.
3. **Bulk Delete Product Options:**
    - Enable Salesman to efficiently manage their inventory by implementing a bulk delete feature for the flowers.
    - Provide a user-friendly interface to select and delete multiple flower options simultaneously.
4. **Coupon & Discount Functionality:**
    - Allow customers to provide a coupon code during checkout.
    - Sellers can input the coupon code, and customers receive a discount based on the coupon.
5. **Duplicate & Edit Feature:**
    - Implement a feature within the product list that includes a button. Upon clicking this button, Salesman will be redirected to a form where product data is pre-filled. Users can then make modifications as needed to create a new product based on the existing one. The button could be named "Duplicate & Edit" or "Create Variant" to convey the idea that users can duplicate an existing product and make modifications to create a new one.
6. **Customer Membership & Points on Purchase:**
    - Introduce a membership system where customers can sign up and earn points on purchases.
    - Assign points based on the purchase amount.
    - Display earned points in the user's profile/dashboard.
    - Implement point redemption functionality for discounts or rewards.
7. **Additional Features:**
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