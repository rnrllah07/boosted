## 🎯 30-Second Elevator Pitch
Boosted is an intuitive online classroom platform tailored for students preparing for UK GCSE English and Math exams. Expert-led live lessons, AI-enhanced content access, and essay feedback—all in a trusted, fully English-language environment with simple subscription pricing.

## 🧩 Problem & Mission
**Problem:** UK students often lack consistent, curriculum-aligned, flexible exam prep for English and Math.

**Mission:** Empower GCSE students with a smart, supportive online system offering:
- Seamless live Zoom-based classes
- Add-on access to AI summaries & lesson replays
- Human-reviewed essay feedback
- Transparent monthly subscriptions

## 🎯 Target Audience
- **Primary:** GCSE students (ages 14–16) in the UK
- **Secondary:** Parents financing tutoring
- **Tertiary:** Qualified Math & English teachers seeking flexible online work

## 🚀 Core Features
- Embedded Zoom-based live classes
- Monthly subscription plans (English / Math / Combo)
- AI-generated lesson summaries & video archive (add-on)
- One-off essay upload + scoring service
- Dynamic student dashboards (class, calendar, status)
- Teacher application, scheduling & feedback workflows
- Admin control panel (classes, users, alerts)
- Stripe-based billing with Apple & Google Pay

## 🏗️ High-Level Tech Stack
- **Frontend:** React (UI components, dashboard)
- **CMS:** Directus (role-based content control)
- **Database:** Supabase (auth, user data, essays)
- **Video:** Zoom SDK (embedded sessions)
- **Payments:** Stripe w/ Google Pay & Apple Pay
- **AI:** GPT-based summarization layer

## 🗂️ Conceptual Data Model
- `User` → roles: student | teacher | admin
- `Class` → subject, time, teacher, Zoom ID, summary
- `Essay` → student upload, feedback, score
- `Subscription` → user, type, status, expiry
- `Add-on` → access to summaries/videos
- `Notification` → system messages

## 🧠 UI Design Principles
- Mobile-first, low-cognitive load, clear actions
- Use of brand blue (#265BF7), white, and black
- Stepper forms, bold buttons, sticky navigation
- Built-in accessibility (AA contrast, focus rings)

## 🔐 Security & Compliance
- GDPR compliant
- Parent info visible only to Super Admins
- 3-device login limit per student
- Stripe secure billing
- On-screen warnings against screen recording

## 🛤️ Roadmap
**MVP**:
- Live classes, auth, Stripe subs, essay upload
**V1**:
- AI summaries, add-on logic, reschedule flow
**V2**:
- Progress tracking, in-app quizzes, post-class ratings

## ⚠️ Risks & Mitigations
- AI accuracy → Teacher-reviewed fallback
- Teacher no-show → Admin alert system
- Churn → Auto-renewal + last-chance reminders

## 🌱 Future Opportunities
- New subjects: Sciences, History
- Parent dashboards
- Essay bundle pricing
- Mobile app

