# Blogflux

Blogflux is a blogging platform that allows users to create, update, and delete blog posts. Users can also rate blogs, comment, and view top blogs and bloggers. The platform features authentication and authorization mechanisms to ensure secure access and interaction.

## API Endpoints

### User Routes
- `GET /users/` - Get all users
- `POST /users/` - Create a new user
- `PATCH /users/` - Update user details (authentication required)
- `DELETE /users/` - Delete a user (authentication required)
- `POST /users/login` - User login
- `GET /users/profile` - Get user profile (authentication required)

### Post Routes
- `GET /post/` - Get all posts
- `POST /post/` - Create a new post (authentication required)
- `PATCH /post/:id` - Update a post (authentication required)
- `DELETE /post/:id` - Delete a post (authentication required)
- `POST /post/like/:id` - Like or unlike a post (authentication required)
- `POST /post/comment/:id` - Create a comment on a post (authentication required)
- `DELETE /post/comment/:postId/:commentId` - Delete a comment (authentication required)
- `GET /post/topblogs` - Get top blogs
- `GET /post/topblogger` - Get top bloggers

## Project Structure
```plaintext
├── config
│   ├── config.js
│   └── db.js
├── controllers
│   ├── posts.controllers.js
│   ├── users.controllers.js
│   └── verifyUser.js
├── models
│   ├── posts.models.js
│   └── users.models.js
├── routes
│   ├── posts.routes.js
│   └── users.routes.js
├── app.js
├── index.js
├── .env
├── package-lock.json
├── package.json
└── README.md
```

### Set up environment variables:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/Blogflux.git
   cd Blogflux 


