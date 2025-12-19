## 🔗 API Endpoints

Base URL: `http://localhost:5000/api`

> Access to endpoints is restricted based on user roles (Faculty, HOD, Admin).

### Authentication Routes
- `POST /api/users/register` – User registration
- `POST /api/users/login` – User login
- `GET /api/users/profile` – Get user profile
- `PUT /api/users/profile/:id` – Update user profile

### Faculty Appraisal Routes
- `POST /api/appraisal-form/submit-appraisal` – Submit new appraisal
- `GET /api/appraisal-form/my-appraisals` – Get faculty appraisals
- `GET /api/appraisal-form/appraisal/:id` – Get specific appraisal
- `PUT /api/appraisal-form/update-appraisal/:id` – Update appraisal  
- PDF generation handled client-side using html2pdf.js

### HOD Routes
- `GET /api/hod/appraisals` – Get department appraisals
- `GET /api/hod/appraisals/:id` – Get specific appraisal details
- `POST /api/hod/review` – Submit HOD review
- `GET /api/hod/dashboard-stats` – Get dashboard statistics
- `GET /api/hod/department-faculty` – Get department faculty list
- `GET /api/hod/reports` – Get HOD reports

### Admin Routes
- `GET /api/admin/appraisals` – Get all appraisals
- `GET /api/admin/appraisals/:id` – Get specific appraisal
- `POST /api/admin/review` – Submit admin review
- `GET /api/admin/dashboard-stats` – Get system statistics
- `GET /api/admin/users` – Get all users
- `PUT /api/admin/users/:id` – Update user details
- `PUT /api/admin/users/:id/role` – Promote user role
- `GET /api/admin/departments` – Get departments list
