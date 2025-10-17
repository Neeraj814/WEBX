 Webx Job Portal Website
Overview

Job Portal Website is a full-stack web application designed to connect job seekers with employers. It provides a seamless platform for posting, searching, and applying for jobs, while also allowing recruiters to find the right talent efficiently.
Features
For Job Seekers:

User registration and authentication

Profile creation and resume upload

Job search with filters (location, salary, skills, etc.)

Apply for jobs directly from the platform

Track application status

Receive job alerts and notifications

For Employers / Recruiters:

Company registration and profile management

Post and manage job listings

View and shortlist applicants

Track application status

For Admin:

Manage users (job seekers & employers)

Approve or reject jobs

Platform analytics and reporting


Technology Stack

Frontend: React.js, Redux, Tailwind CSS, React Router,shadnui
Backend: Node.js, Express.js
Database: MongoDB
Authentication: JWT
Hosting: Render

Database Schema

User
fullname : String
email : String (unique)
phoneNumber : Number (10+ digits)
role : String (job seeker / recruiter / admin)
password : String
resume : File / URL
appliedJobs : Array of Job IDs

Job
title : String
description : String
location : String
salary : String
companyId : ObjectId
applicants : Array of User IDs

Company
name : String
description : String
jobsPosted : Array of Job IDs

Application
jobId : ObjectId
userId : ObjectId
status : String (applied / shortlisted / rejected)

Installation
1. Clone the repository:
  git clone https://github.com/yourusername/job-portal.git
  cd job-portal
2.Install dependencies:
 npm install
3. Create .env file with required variables:
   PORT=5000
   MONGO_URI=your_mongodb_uri
   JWT_SECRET=your_jwt_secret
4. Run the backend:
   npm run dev
5. npm start

Folder Structure
job-portal/
├─ backend/
│  ├─ models/
│  ├─ routes/
│  ├─ controllers/
│  └─ server.js
├─ frontend/
│  ├─ src/
│  │  ├─ components/
│  │  ├─ pages/
│  │  └─ App.js
├─ README.md
└─ package.json


Contributing

Fork the repository
Create a new branch: git checkout -b feature/your-feature
Commit your changes: git commit -m "Add new feature"
Push to the branch: git push origin feature/your-feature
Create a Pull Request

License
This project is licensed under the MIT License.
