# Product Management Application

This project is a web-based product management application that allows users to manage product data in a Snowflake database. The application provides functionalities for querying products, uploading files, executing tasks, clearing stages, truncating tables, and adding, editing, and deleting products.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Query Products**: Fetch and display product data from the Snowflake database.
- **Upload Files**: Upload files to Snowflake stages for data loading.
- **Execute Task**: Trigger Snowflake tasks to process data.
- **Clear Product Stages**: Remove files from Snowflake stages.
- **Truncate Product Table**: Clear all data from the product table.
- **Add Product**: Add new product entries to the database.
- **Edit Product**: Update existing product details (coming soon).
- **Delete Product**: Remove product entries from the database.

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (Flask)
- **Database**: Snowflake
- **APIs**: Fetch API for frontend-backend communication

## Setup and Installation

### Prerequisites

- Python 3.x
- Node.js and npm
- Snowflake account

### Backend Setup

1. **Clone the repository**:

    ```bash
    git clone https://github.com/your-repo/product-management-app.git
    cd product-management-app
    ```

2. **Create a virtual environment and activate it**:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:

    Create a `.env` file in the root directory with the following content:

    ```env
    SNOWFLAKE_USER=<your_snowflake_user>
    SNOWFLAKE_PASSWORD=<your_snowflake_password>
    SNOWFLAKE_ACCOUNT=<your_snowflake_account>
    SNOWFLAKE_WAREHOUSE=<your_snowflake_warehouse>
    SNOWFLAKE_DATABASE=<your_snowflake_database>
    SNOWFLAKE_SCHEMA=<your_snowflake_schema>
    SNOWFLAKE_ROLE=<your_snowflake_role>
    ```

5. **Run the Flask application**:

    ```bash
    python app.py
    ```

### Frontend Setup

1. **Navigate to the `frontend` directory**:

    ```bash
    cd frontend
    ```

2. **Install dependencies**:

    ```bash
    npm install
    ```

3. **Run the application**:

    ```bash
    npm start
    ```

## Usage

1. **Open the application in your browser**:

    Navigate to `http://localhost:5000` to access the application.

2. **Use the sidebar buttons**:

    - **Query Products**: View a list of products from the database.
    - **Upload to Stage**: Upload a file to a Snowflake stage.
    - **Execute Task**: Trigger a Snowflake task.
    - **Clear Product Stages**: Remove all files from Snowflake stages.
    - **Truncate Product Table**: Clear all data from the product table.
    - **Add Product**: Open the form to add a new product.

3. **Perform CRUD operations**:

    Use the "Edit" and "Delete" buttons in the product table rows to manage products.

## API Endpoints

- `POST /uploadToStage`: Upload a file to Snowflake stage.
- `POST /executeTask`: Execute a Snowflake task.
- `GET /queryProducts`: Retrieve product data from the database.
- `POST /addProduct`: Add a new product to the database.
- `POST /deleteProduct`: Delete a product from the database.
- `POST /clearProductStages`: Clear all Snowflake stages.
- `POST /truncateProductTable`: Truncate the product table.

## Contributing

Feel free to fork the repository and submit pull requests. For major changes or features, please open an issue to discuss your ideas.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to adjust any sections to better fit your project’s specifics!
