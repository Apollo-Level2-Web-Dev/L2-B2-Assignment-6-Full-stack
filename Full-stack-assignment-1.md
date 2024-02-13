## Electric gadgets **Management Dashboard with Role System and Cart Functionality**

Each product must have following information

- Product name
- Product price
- Product quantity
- Product Image (You can use image link or use any third-party image hosting provider like ImgBB to host your product images)

**Note: Additionally, ensure to include more product information based on the specified filter criteria mentioned in point 3.**

## **Requirements:**

**Objective:**
The primary objective of this assignment is to design and implement a comprehensive Electric gadgets Management Dashboard, providing the tools to efficiently manage the Electric gadgets inventory, track sales, and analyze sales history. The assignment will incorporate features such as authentication, CRUD operations, state management, real-time UI updates, and Electric gadgets filtering.

**Authentication:**

1. **User Registration and Login:**
    - Users must register and log in to access the dashboard.
    - Use JWT (JSON Web Tokens) for secure authentication.
    - Roles:
        1. **User Role:**
            - Users with the role of "User" have restricted access compared to managers. They can only modify the products they have added to the inventory. This means they can perform CRUD (Create, Read, Update, Delete) operations exclusively on the products they own.
            - Specifically, a user can:
                - Add new books to the inventory.
                - Delete their existing books from the inventory.
                - Update details of the books they have added.
                - View and read the list of books they have added.
        2. **Manager Role:**
            - Users with the role of “Manager” have broader permissions and can modify any product within the inventory. This role is typically assigned to administrators or higher-level staff members responsible for overseeing the entire inventory.
            - Managers can perform all CRUD operations on any product in the inventory, regardless of who added it. This includes:
                - Adding new books to the inventory.
                - Deleting existing books from the inventory.
                - Updating details of any book in the inventory.
                - Viewing and reading the list of all books in the inventory.
        
        By defining these roles and their respective permissions, the system ensures that users have control and ownership over the products they add while allowing managers to oversee and manage the entire inventory efficiently.
        

**Functionality:**

1. Electric gadgets **Management:**
    - CRUD Operations:
        - Add a new Electric gadgets to the inventory.
        - Delete existing Electric gadgets from the inventory.
        - Update Electric gadgets details.
        - Read and view the list of Electric gadgets in the inventory.
        - Implement a robust filtering system to effectively narrow down Electric gadgets selections based on various criteria.
2. **Sales History:**
    - View sales history categorized by:
        - Weekly
        - Daily
        - Monthly
        - Yearly
3. **Filtering (Implement on the** Electric gadgets **management page)**
- Design a robust filter system tailored for electric gadgets to streamline inventory management and facilitate customer searches. The filter options should be aligned with the unique characteristics of electronic devices:
    - **Filter by Price Range:** Allow users to set a specific price range for electric gadgets.
    - **Filter by Release Date:** Provide options for filtering gadgets based on their release date or model year.
    - **Filter by Brand:** Implement a real-time search functionality for brand names to quickly identify and manage gadgets from specific manufacturers.
    - **Filter by Model Number:** Enable searching by unique model numbers for precise identification.
    - **Filter by Category:** Categorize gadgets into types (e.g., smartphones, laptops, cameras) and allow filtering by these categories.
    - **Filter by Operating System:** If applicable, provide options to filter gadgets based on the operating system they use (e.g., iOS, Android, Windows).
    - **Filter by Connectivity:** Allow users to filter gadgets based on connectivity options (e.g., Bluetooth, Wi-Fi, USB-C).
    - **Filter by Power Source:** Include options to filter gadgets based on their power source (e.g., battery-powered, plug-in).
    - **Filter by Features:** Introduce filters for specific features like camera resolution, storage capacity, screen size, or any other relevant specifications.
    - **Additional Relevant Filter Parameters:** Customize the filter options further based on the specific attributes and functionalities of electric gadgets, such as weight, dimensions, or compatibility with certain accessories.
1. **User Interface Features:**
    - Gracefully update the UI in real-time when changes occur (e.g., product updates, sales, etc.).
    - Utilize RTK Query for efficient CRUD operations.
    - Implement **Re-fetching** functionality to ensure data accuracy and consistency.
2. **State Management:**
    - Utilize Redux for state management to maintain a consistent application state.
3. **Bulk Delete Product Options:**
    - Enable user to efficiently manage their inventory by implementing a bulk delete feature for the Electric gadgets.
    - Provide a user-friendly interface to select and delete multiple Electric gadgets options simultaneously.
4. Implement a feature within the product list that includes a button. Upon clicking this button, users will be redirected to a form where product data is pre-filled. Users can then make modifications as needed to create a new product based on the existing one. The button could be named "Duplicate & Edit" or "Create Variant" to convey the idea that users can duplicate an existing product and make modifications to create a new one.
5. **Cart System:**
    - Users with the roles of "Manager" or "User" have the capability to add products to the cart.
    - Each product card will feature an "Add to Cart" button for adding the product tot he cart.
    - The "Add to Cart" button will dynamically respond: if the product is already present in the cart, the button will become disabled, preventing duplicate entries.
6. Checkout page:
    - Upon reaching the checkout page, users, both managers and regular users, will encounter a summary of their cart contents along with the respective quantities of each product added.
    - The checkout page will dynamically calculate and display the total amount based on the quantities of products in the cart and their corresponding prices.
    - Users will have the ability to increase or decrease the quantities of products in the cart directly from the checkout page, ensuring a seamless and intuitive shopping experience. Quantity of the product to be sold cannot exceed the current available stock of the product.
        - **Note: If the quantity reaches zero after selling a product, the product will be removed from the inventory.**
    - Additionally, users will be able to remove products entirely from the cart if they decide not to sell any product.
    - Alongside the cart summary, there will be a section for users to input essential information for the sale transaction. This section will include fields for the buyer's name, contact number, and the selling date, ensuring accurate record-keeping and facilitating smooth transactions.
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
- You can create the backend for this assignment in a single page, but but we highly recommend applying the modular pattern we introduced in Level 2 for enhanced code organization and maintainability.

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
