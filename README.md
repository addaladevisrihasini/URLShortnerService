# 🔗 URL Shortener Service  

When sharing links on LinkedIn, resumes, or social media, long URLs often look cluttered, unprofessional, and difficult to read.  
A **URL Shortener Service** solves this problem by converting long, complex URLs into short, user-friendly links.  

✅ **Example:**  
https://www.example.com/articles/2025/08/22/url-shortener-service-documentation 👉 Becomes:  
https://short.ly/url-doc (where `url-doc` is the input given by the user)  

This makes links easier to **share, remember, and customize**.  

---

## 🚀 Features  
- Shortens long URLs into easy-to-share links  
- Allows **custom aliases** (e.g., `short.ly/myresume`)  
- Provides **optional click tracking & analytics**  
- Prevents broken or mistyped links  
- Perfect for **resumes, portfolios, LinkedIn, or project demos**  

---

## 🔗 Custom Alias Example  
Instead of random IDs like `abc123`, users can choose their own alias:  
- https://short.ly/myportfolio  
- https://short.ly/devprofile  

---

## 📖 Conclusion  
The **URL Shortener Service** is a simple yet powerful tool that makes long URLs more **professional, shareable, and user-friendly**.  

It is especially useful for:  
- **Resumes**  
- **LinkedIn posts**  
- **Portfolios**  
- **Project demos**  

💡 With **custom aliases, analytics, and QR codes**, it can evolve into a **production-grade service**.  

---

# 🐳 Running with Docker  

This project includes a `Dockerfile` so you can run it easily inside a container.  

---

##🔹 For Other Developers (Pull & Run Image)
### 1. Login to Docker Hub:
   ```bash
        docker login
   ```
### 2. Pull the image from Docker Hub:
 ```bash
        docker pull rishithakoganti/url-shortner-server:latest

```
### 3. Run the container and the env file:
 ```bash
       docker run --env-file backend/.env -p 5000:5000 rishithakoganti/url-shortner-server:latest
```
### 4. Check running containers:
```bash
         docker ps
```
### 5. View container logs (optional):
```bash
         docker logs -f url-shortener-container
```
✅ Now the service will be running at:
👉 http://localhost:5000/ (or the port you exposed)

---
**✨ Members’ Contribution Summary**
**👩‍💻 Rishitha Koganti (23211A6751)**

Contributed to project integrates a static frontend built with HTML, CSS, and Bootstrap with a backend powered by Node.js and Express. The frontend provides the user interface, while the backend handles API requests, server logic, and external integrations.


**Frontend–Backend Integration**

The frontend consists of responsive pages styled with Bootstrap.
All dynamic requests (such as URL shortening) are sent to the backend through defined API routes.
In production, the backend is configured to serve both the frontend files and API from the same server, ensuring smooth operation without CORS issues.

**Bitly Key Integration and Verification**

A Bitly Access Token is used to enable URL shortening.
The key is stored as an environment variable in the backend for security.
When the server starts, the key is verified with the Bitly API to ensure it is valid.
The backend exposes a secure endpoint for shortening 

**Dockerfile and Deployment**

The project includes a Dockerfile for seamless deployment.
It defines instructions to copy the project files, install dependencies, and configure the server.
The frontend static files are bundled with the backend so the application runs in a single container.
Environment variables such as the Bitly key are passed at runtime for better security.
A healthcheck ensures that the containerized application is running correctly.
Deployment is simplified, portable, and production-ready using Docker.

 **👩‍💻 Navya Sree (23211A6710)**
 
**Frontend Styling**

		Designed and customized the user interface (UI) with advanced CSS styling, ensuring the application has a clean, modern, and visually appealing look.
		Focused on making the frontend responsive across multiple screen sizes, ensuring a smooth experience on desktops, tablets, and mobile devices.
		Enhanced user experience (UX) by refining layouts, improving typography choices, adjusting spacing, and aligning elements consistently to create a professional flow throughout the             application.
		Worked on improving visual hierarchy and readability, making navigation more intuitive for end-users.
**Backend Integration**

		Integrated the application with MongoDB to store and manage user authentication details securely.
		Implemented login and signup functionalities, ensuring proper encryption and validation of sensitive data like passwords.
		Designed and maintained an efficient database schema to handle user-related data without redundancy, enabling faster query execution and smoother performance.
		Ensured proper error handling and data validation in backend routes to increase reliability and prevent faulty user input.
**API Integration**

		Successfully integrated the Bitly API to add URL shortening functionality, allowing users to generate shorter, shareable links directly from the application.
		Created and configured a new Bitly API token, which was carefully stored as an environment variable to enhance project security and prevent accidental exposure.
		Implemented API request handling in the backend, verifying responses from the Bitly API to confirm reliability and validity.
		Tested the integration thoroughly to ensure smooth performance and handled edge cases such as invalid or expired tokens gracefully.
**Deployment**

		Deployed the complete full-stack application on Render, making it accessible to users with a stable and secure hosting environment.
		Configured production-ready connections between the backend, frontend, and MongoDB database to ensure data flow remains uninterrupted after deployment.
		Optimized deployment by managing environment variables, including the Bitly token, to ensure security and scalability.
		Conducted multiple validation checks post-deployment to confirm that authentication, API integration, and overall application functionalities worked seamlessly in the live environment.
		Ensured the deployed version of the project delivers a real-world ready solution with consistent uptime and reliability.
**👩‍💻 Vyshnavi (23211A6721)**

Backend Development from Scratch
	•	Designed and developed the backend architecture completely from scratch using Node.js and Express, ensuring a clean, modular, and scalable codebase.
	•	Defined proper folder structures, routes, middleware, and controllers to maintain code readability and separation of concerns.
	•	Implemented server-side logic to handle all major functionalities of the project, including API routing, data validation, and error handling.
	•	Focused on performance optimization by ensuring efficient query handling, middleware usage, and structured workflows in the backend.
	•	Added proper logging and debugging mechanisms to monitor backend operations during both development and deployment.

Authentication System
	•	Built a secure authentication system using MongoDB for storing and managing user credentials.
	•	Implemented user registration and login features with validation and error handling.
	•	Ensured password security by applying encryption/hashing techniques before storing in the database.
	•	Created middleware functions to verify authentication tokens and restrict access to protected routes.
	•	Designed the system to handle session management and ensure secure access across the application.

URL Shortening Functionality
	•	Developed the backend logic for short link generation, integrating the Bitly API for accurate and reliable shortening.
	•	Created endpoints to receive long URLs from the frontend and return shortened URLs as output.
	•	Configured and managed the Bitly API token securely using environment variables, preventing token leakage.
	•	Implemented response validation and error handling to manage cases such as invalid URLs or expired tokens.
	•	Optimized backend responses to ensure the short link output is returned quickly and accurately for end-users.

End-to-End Backend Responsibility
	•	Took ownership of building, testing, and debugging the backend system end-to-end.
	•	Ensured that both authentication and URL shortening features were thoroughly tested and working seamlessly.
	•	Collaborated with team members to integrate backend APIs with the frontend interface, ensuring smooth data exchange.
	•	Delivered a reliable, production-ready backend that supports all major functionalities of the project.

**🌍 Live Deployment**

🔗 Website is live here: 👉 https://urlshortnerservice-backend-6euz.onrender.com

⚠️ Caution: The free Bitly API key allows only 3 shorten requests. If you exceed this limit, you’ll see an error like: Failed to shorten URL - API limit exceeded.






