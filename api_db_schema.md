## 🔌 API Endpoints for Boosted

### 🔐 Auth
- `POST /auth/signup`
- `POST /auth/login`
- `GET /auth/me`
- `PUT /profile/update`

### 🧾 Subscriptions
- `POST /subscriptions/start`
- `GET /subscriptions/status`
- `POST /subscriptions/cancel`

### 🗓️ Classes
- `GET /classes?user_role=student`
- `GET /classes?user_role=teacher`
- `POST /classes/reschedule-request`
- `POST /classes/start`
- `GET /classes/:id`

### 📄 Essays
- `POST /essays/upload`
- `GET /essays/by-user`
- `POST /essays/:id/review`

### 📼 AI Summaries
- `GET /videos/:class_id`
- `POST /summaries/generate`
- `GET /summaries/free-used`

### 🔔 Notifications
- `GET /notifications`
- `POST /notifications/mark-read`

---

## 🗂️ Database Schema Overview

### `users`
- id (UUID)
- role (student | teacher | admin)
- name, email, password_hash
- GCSE level, profile info, parent contact (if student)

### `subscriptions`
- id, user_id → users
- type (english | math | combo)
- start_date, end_date
- status (active | cancelled)

### `classes`
- id, subject, teacher_id → users
- scheduled_time
- zoom_session_id
- ai_summary_id (nullable)

### `essays`
- id, student_id → users
- upload_link
- reviewer_id → users
- score, comment

### `ai_summaries`
- id, class_id → classes
- summary_text, keywords, created_at

### `add_ons`
- id, user_id → users
- valid_from, valid_until
- type (video_archive)

### `notifications`
- id, user_id
- type (system | essay | subscription)
- message, read_at

