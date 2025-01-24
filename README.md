# Blog Application

A blog application that allows users to create, read, update, and delete (CRUD) blog posts. The project consists of a backend API server and a frontend server for rendering views and interacting with the API.

---

## Project Structure

```bash

project 
├── public 
│ └── styles 
│  └── main.css # Stylesheet for the application 
├── views 
│ ├── index.ejs # Main page to display blog posts 
│ ├── modify.ejs # Page for creating or editing blog posts 
├── index.js # Backend API server (CRUD functionality) 
├── server.js # Frontend server (renders views and handles interactions) 
└── README.md # Project documentation

```


---

## Features

1. **Create New Blog Posts**  
   Users can create blog posts with a title, content, and author.

2. **View All Blog Posts**  
   Displays a list of all blog posts on the main page.

3. **Edit Blog Posts**  
   Allows editing of existing blog posts.

4. **Delete Blog Posts**  
   Users can delete blog posts from the application.

5. **Responsive Design**  
   Styled for a seamless user experience across different devices.

---

## Technologies Used

- **Frontend:**
  - EJS (Embedded JavaScript Templates)
  - CSS

- **Backend:**
  - Node.js
  - Express.js
  - Axios (for API communication)

---

## Setup Instructions

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/Mech-Kal/blog-application.git
   cd blog-application
   ```
2. **Install Dependencies**
    Install the required dependencies for both servers:

    ```bash
    npm install
    ```
3. **Run the Backend API Server**
    Open a terminal and start the API server:

    ```bash
    node index.js
    The API server will run on http://localhost:4000.
    ```
4. **Run the Frontend Server**
    Open another terminal and start the frontend server:

    ```bash
    node server.js
    The frontend server will run on http://localhost:3000.
    ```

5. **Access the Application**
    Open your browser and visit:
    ```bash
    http://localhost:3000
    ```
---
## API Endpoints

The backend API (`index.js`) exposes the following endpoints:

| **Method** | **Endpoint**    | **Description**                     |
|------------|-----------------|-------------------------------------|
| GET        | `/posts`        | Fetch all blog posts                |
| GET        | `/posts/:id`    | Fetch a specific blog post by ID    |
| POST       | `/posts`        | Create a new blog post              |
| PATCH      | `/posts/:id`    | Update an existing blog post        |
| DELETE     | `/posts/:id`    | Delete a blog post by ID            |
---

## Development Workflow

1. Frontend Development
- Modify `views/index.ejs` and `views/modify.ejs` for UI changes.
- Update `public/styles/main.css` for styling.

2. Backend API Development
- Update `index.js` to modify or extend API functionality.

3. Frontend-Backend Integration
- Use `axios` in `server.js` to fetch or send data between the frontend and API.

---

## Usage

1. **Create a New Blog Post**
- Navigate to `/new` or click "New Post" on the homepage.
- Fill in the form and submit to add the post.

2. **Edit a Blog Post**
- Click the "Edit" button on a post.
- Update the form fields and submit to save changes.

3. **Delete a Blog Post**
- Click the "Delete" button on a post to remove it from the database.

4. **View Blog Posts**
- Posts are listed on the homepage with their title, content, and author.
