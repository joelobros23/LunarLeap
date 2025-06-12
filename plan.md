# Project Plan: LunarLeap

**Description:** A streamlined web hosting platform providing domain management and basic server control features, built on Ruby on Rails with SQLite3, Tailwind CSS, and Devise.


## Development Goals

- [ ] Configure tailwindcss-rails and apply basic Tailwind styling to the application layout (application.html.erb).
- [ ] Implement user authentication using Devise: Configure routes and views to handle user registration, login, and logout.
- [ ] Modify the Domain model to include validations for `name`, `plan`, and `user_id` presence. Also, add a unique index on the domain name to prevent duplicates.
- [ ] In the Domains controller, ensure that only logged-in users can create, edit, or delete their own domains. Use `before_action` filters and `current_user` to achieve this.
- [ ] Customize the domains index view (index.html.erb) to display domains belonging only to the currently logged-in user.
- [ ] Implement domain status management. Add functionality to change the status of a domain (e.g., 'active', 'inactive', 'suspended').  Consider using an enum or a simple string field.
- [ ] Design and implement different hosting plans (e.g., 'Basic', 'Standard', 'Premium') with associated features and limitations.
- [ ] Implement a basic dashboard for users to view their domains, account information, and recent activity.
- [ ] Add basic error handling and display user-friendly error messages for common issues like invalid domain names or insufficient permissions.
- [ ] Implement a simple contact form using Action Mailer that will allow users to submit support requests.
