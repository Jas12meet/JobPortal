# JobPortal – Full-Stack Job Recruitment Platform

**Project Overview**

JobPortal is a full-stack web application developed using the MERN stack (MongoDB, Express.js, React.js, and Node.js) that connects job seekers with recruiters through a centralized platform. It allows users to register and log in, browse job opportunities, apply for jobs, and track their application status. Recruiters can access role-specific functionality for managing job postings and applications. The platform aims to simplify the recruitment process by providing a responsive interface, secure authentication, role-based authorization, and organized application tracking.

**System Architecture**

The application follows a client-server architecture with three primary layers:

1. **Frontend:** Built with React.js and Vite, styled using Tailwind CSS. It provides the user interface for registration, login, job browsing, job applications, and application status tracking.
2. **Backend:** Built with Node.js and Express.js, it handles HTTP requests, implements application logic, enforces authentication and authorization, and exposes RESTful APIs for user management, job postings, and application tracking.
3. **Database and Media Storage:** MongoDB stores application data, with Mongoose managing database schemas and interactions. Multer and Cloudinary support profile picture and document uploads.

The frontend communicates with the backend through RESTful APIs, while the backend interacts with MongoDB to persist and retrieve information.

**Technology Stack and Implementation Details**

- **React.js and Vite:** React provides a component-based frontend architecture, enabling reusable UI components and easier maintenance. Vite provides the development and build tooling for the frontend.
- **Tailwind CSS:** Used to style the application and build a responsive, consistent interface across different screen sizes.
- **Node.js:** Provides the JavaScript runtime for executing backend code and handling application requests.
- **Express.js:** Used to create backend routes and RESTful APIs for user management, job postings, and application tracking.
- **MongoDB:** A NoSQL database used to store application data. Its flexible document structure is suitable for representing user profiles, job details, and application information.
- **Mongoose:** Provides schema definitions, data validation capabilities, and a structured way to interact with MongoDB from the Node.js backend.
- **JWT (JSON Web Tokens):** Used to authenticate users and support protected routes by verifying their identity through signed tokens.
- **bcrypt:** Used to hash passwords before storage, rather than saving passwords as plain text.
- **Multer and Cloudinary:** Multer handles incoming file uploads on the backend, while Cloudinary provides cloud-based storage and delivery for profile pictures and documents.
- **RESTful APIs:** Establish a clear communication interface between the frontend and backend, separating user-interface concerns from server-side business logic.
- **Render:** Used to deploy the application for testing and gathering user feedback.

**Core Functional Components**

1. **User Authentication:** Users can register and log in through an authentication flow using JWT and bcrypt.
2. **Role-Based Access Control:** Students/job seekers and recruiters have role-specific access. Protected routes and backend authorization checks help restrict functionality to permitted users.
3. **Job Management:** RESTful endpoints support job-posting operations, enabling the platform to manage job-related information.
4. **Job Applications:** Job seekers can apply for jobs, and the application system supports tracking the status of submitted applications.
5. **Application Status Tracking:** Users can view whether their applications have been accepted or rejected.
6. **Profile and Document Uploads:** Multer and Cloudinary are integrated to handle profile pictures and document uploads.
7. **Responsive User Interface:** React and Tailwind CSS provide an accessible, user-friendly interface for interacting with the platform.

**Key Design Decisions**

- **MERN stack:** Using JavaScript across the frontend and backend simplifies development and allows code and data structures to remain consistent across application layers.
- **MongoDB with Mongoose:** A document-oriented database offers flexibility for job listings, user profiles, and application records, while Mongoose adds schema-based organization.
- **RESTful API architecture:** Separating frontend and backend responsibilities makes endpoints easier to maintain, test, and extend.
- **JWT and bcrypt:** JWT supports authenticated requests, while bcrypt protects stored passwords through hashing.
- **Role-based authorization:** Separating job-seeker and recruiter permissions helps prevent unauthorized access to role-specific operations.
- **Cloudinary integration:** Storing uploaded media in a dedicated cloud service avoids relying exclusively on the application server's local filesystem.
- **React with Vite and Tailwind CSS:** This combination supports reusable frontend components, efficient development, and responsive styling.

**Testing and Deployment**

The application was deployed on Render for testing and user feedback. The project uses RESTful APIs for communication between the frontend and backend, and the backend integrates with MongoDB through Mongoose. API testing and debugging can be performed using tools such as Postman; however, include Postman in the project's testing process only if you actually used it for this project.

**Conclusion**

JobPortal demonstrates full-stack web development by combining frontend development, backend API design, database integration, authentication, role-based access control, file uploads, and deployment. The project provides practical experience in building a complete web application in which users can interact with job listings and manage recruitment-related activities through a centralized platform.
