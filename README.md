# WriteFlow🍃: AI-Enabled Full Stack Blog Platform

<img width="1827" height="842" alt="image" src="https://github.com/user-attachments/assets/05bae76d-f630-4482-be4d-8b77d593ac47" />


## Overview

WriteFlow is a modern, full-stack blogging platform built using the **MERN stack** (MongoDB, Express.js, React, Node.js). Integrated with **Google Gemini** for AI-powered content generation and **ImageKit** for efficient image management, WriteFlow offers a seamless experience for creating, managing, and publishing blogs. The platform includes a robust **admin dashboard** for managing posts and comments, and is deployed online using **Vercel** for scalability and performance.

This project showcases a complete end-to-end solution for a blog application, combining a dynamic frontend, a secure backend, and AI-driven content creation capabilities. Whether you're a developer looking to learn full-stack development or a content creator seeking an intuitive blogging platform, WriteFlow has you covered.

---

## Features

- **AI-Powered Content Generation** : Leverage Google Gemini to generate engaging blog content effortlessly.
- **Admin Dashboard** : Manage blog posts and comments with an intuitive, secure interface.
- **Image Management** : Upload and optimize blog images using ImageKit API.
- **Responsive Design** : A mobile-friendly interface built with React for a seamless user experience.
- **Secure Authentication** : Robust login system for admin access.
- **CRUD Operations** : Create, read, update, and delete blog posts and comments via RESTful APIs.
- **Scalable Deployment** : Deployed on Vercel for high availability and performance.
- **MongoDB Integration** : Efficient data storage and retrieval for blogs and comments.

---

## Tech Stack

- **Frontend** : React.js, Tailwind CSS
- **Backend** : Node.js, Express.js
- **Database** : MongoDB
- **AI Integration** : Google Gemini API
- **Image Management** : ImageKit API
- **Deployment** : Vercel
- **Other Tools** : Axios, JWT for authentication, bcrypt for password hashing

---

## Project Structure

```
WriteFlow/
├── client/                     # React frontend
│   ├── src/
│   │   ├── components/         # Reusable React components
│   │   ├── pages/              # Home, Blog, Admin Dashboard pages
│   │   ├── assets/             # Static assets (images, styles)
│   │   └── App.js              # Main React app component
├── server/                     # Node.js/Express backend
│   ├── routes/                 # API routes (auth, blogs, comments)
│   ├── models/                 # MongoDB schemas
│   ├── controllers/            # API logic
│   ├── middleware/             # Authentication middleware
│   └── server.js               # Main server file
├── README.md                   # Project documentation
└── package.json                # Project dependencies
```

---

## Installation

Follow these steps to set up WriteFlow locally:

### Prerequisites

- Node.js (v16 or higher)
- MongoDB (local or MongoDB Atlas)
- ImageKit account and API keys
- Google Gemini API key
- Vercel account for deployment

### Steps

1. **Clone the Repository** :

```bash
   git clone https://github.com/ShaktiPriya/WriteFlow.git
   cd WriteFlow
```

1. **Install Dependencies** :

- For the frontend:
  ```bash
  cd client
  npm install
  ```
- For the backend:
  ```bash
  cd server
  npm install
  ```

1. **Set Up Environment Variables** :

- Create a `.env` file in the `server` directory:
  ```env
  MONGO_URI=your_mongodb_connection_string
  JWT_SECRET=your_jwt_secret
  IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
  IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
  GEMINI_API_KEY=your_gemini_api_key
  ```

1. **Run the Application** :

- Start the backend server:
  ```bash
  cd server
  npm start
  ```
- Start the frontend:
  ```bash
  cd client
  npm start
  ```

1. **Access the App** :

- Frontend: `http://localhost:3000`
- Backend APIs: `http://localhost:5000`

---

## Usage

### For Users

- **Browse Blogs** : Visit the homepage to explore published blog posts.
- **Read Blogs** : Click on a blog to view its details and leave comments.
- **AI-Generated Content** : Admins can generate blog content using the integrated Google Gemini API.

### For Admins

- **Login** : Access the admin dashboard using secure credentials.
- **Manage Blogs** : Create, update, or delete blog posts via the dashboard.
- **Manage Comments** : Moderate user comments on blog posts.
- **Image Uploads** : Upload and optimize images using ImageKit.

---

## API Endpoints

### Authentication

- `POST /api/auth/login`: Admin login
- `POST /api/auth/register`: Admin registration (optional)

### Blog Posts

- `POST /api/blogs`: Create a new blog post
- `GET /api/blogs`: Fetch all blog posts
- `GET /api/blogs/:id`: Fetch a specific blog post
- `PUT /api/blogs/:id`: Update a blog post
- `DELETE /api/blogs/:id`: Delete a blog post

### Comments

- `POST /api/comments`: Add a comment to a blog post
- `GET /api/comments/:blogId`: Fetch comments for a blog post
- `DELETE /api/comments/:id`: Delete a comment

### Admin Dashboard

- `GET /api/admin/dashboard`: Fetch dashboard data (blogs, comments, stats)

---

## Deployment

WriteFlow is deployed on **Vercel** for high availability. To deploy your own instance:

1. Push your code to a GitHub repository.
2. Connect the repository to Vercel.
3. Set up environment variables in Vercel’s dashboard.
4. Deploy the frontend (`client`) and backend (`server`) as separate Vercel projects.
5. Configure the backend API URL in the frontend’s environment variables.

Visit the deployed app: [WriteFlow on Vercel](https://writeflow.vercel.app/) _(update with your deployed URL)_

---

## Screenshots

### Admin Login

![Uploading image.png…]()


### Blog Page

<img width="1137" height="865" alt="image" src="https://github.com/user-attachments/assets/3c677cf3-7774-4043-97c9-cee8657e2e29" />


### Admin Dashboard

<img width="1844" height="792" alt="image" src="https://github.com/user-attachments/assets/af78a0fc-1766-42cd-aa2f-7a89061c0b86" />

### Content Generation with AI

<img width="798" height="804" alt="image" src="https://github.com/user-attachments/assets/75448c1d-e372-4993-bc68-81b51f155277" />


---

## Contributing

Contributions are welcome! To contribute to WriteFlow:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature`.
3. Make your changes and commit: `git commit -m "Add your feature"`.
4. Push to the branch: `git push origin feature/your-feature`.
5. Open a pull request.

Please ensure your code follows the project’s coding standards and includes appropriate tests.

---

## License

This project is licensed under the **MIT License** . See the [LICENSE](https://grok.com/chat/LICENSE) file for details.

---

## Author

**ShaktiPriya**

- GitHub: [github.com/ShaktiPriya](https://github.com/ShaktiPriya)
- Email: shaktipriya@example–

.com

- LinkedIn: [linkedin.com/in/shaktipriya](https://linkedin.com/in/shaktipriya)

---

## Acknowledgments

- **Google Gemini** : For powering AI content generation.
- **ImageKit** : For efficient image management and optimization.
- **Vercel** : For seamless deployment and hosting.
- **MongoDB** : For a robust and scalable database solution.
- **MERN Stack Community** : For the amazing tools and libraries.

---

Happy Blogging with WriteFlow! 🚀
