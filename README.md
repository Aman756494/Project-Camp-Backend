A backend REST API for a project management app (a mini Basecamp/Trello), written in Node.js, Express 5 and MongoDB (Mongoose). It has no frontend yet. It includes:

Authentication: register, login, logout, JWT access and refresh tokens stored in cookies, email verification, forgot/reset password, and change password. Emails go out through Nodemailer and Mailgen (Mailtrap for testing).
Projects: create, read, update and delete projects, plus adding members to a project.
Roles and permissions: each project member has a role (admin, project_admin or member), and a middleware checks the role before allowing an action.
Tasks and subtasks: data models and a few controllers exist, but most of the task code is unfinished.
Supporting pieces: request validation (express-validator), a standard response and error format, an async error wrapper, file upload setup (multer), and a health check.