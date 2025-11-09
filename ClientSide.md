# File: client/src/App.jsx

Functions:

Initializes the main React Router setup for the entire frontend.

Manages global authentication state using React hooks (useState, useEffect).

Decodes JWT tokens from localStorage to extract user information (role, email, department).

Controls login and logout behavior via handleLoginSuccess() and handleLogout().

Implements protected routing logic to restrict access based on user roles:

Students & Staff → Complaint pages

Admins → Admin dashboard

Unauthorized users → Redirected to appropriate login pages

Renders the Navbar dynamically based on login state and user role.

Key Points:

Uses React Router DOM (BrowserRouter, Route, Switch, Redirect) for navigation control.

Uses jwt-decode to parse token and maintain persistent login.

Protects role-based routes:

/admin/dashboard → Admin only

/staff/dashboard → Staff only

Complaint routes → Students/Staff only

Stores authentication details (token, user info) in localStorage for persistence.

Centralizes all route definitions and redirection logic in one file for better maintainability.

Redirects users dynamically after login depending on their role.