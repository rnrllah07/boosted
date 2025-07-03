## 🛠️ Implementation Plan for Boosted

### ✅ Phase 1 – MVP
1. **Landing Page**
   - Brand intro, package cards, testimonials, FAQ
2. **Auth System**
   - Google/email login + profile stepper (GCSE info, parent info)
3. **Role-Based Dashboards**
   - Student: calendar, join buttons, dashboard
   - Teacher: class list, reschedule requests
   - Admin: schedule management, teacher approval
4. **Zoom SDK Integration**
   - Embed live class view
   - Teacher triggers session; student joins via dashboard
5. **Stripe Subscriptions**
   - 3 plans: English, Math, Combo
   - Auto-renew, cancellation, device limit logic
6. **Essay Upload**
   - Upload form, teacher review screen, score + feedback delivery

### 🚀 Phase 2 – V1
7. **AI Summary Module**
   - Triggered summary from past classes
   - Conditional access (add-on check)
   - One-time free preview system
8. **Add-On System**
   - Stripe-based single add-on purchase
   - Expiry logic + content restriction
9. **Admin Enhancements**
   - Conflict alerts, KPI dashboard
   - Weekly expiring plans email
10. **Teacher Rescheduling**
   - Request & admin approval workflow

### 🔮 Phase 3 – V2
11. **Student Analytics**
   - Attendance, AI use, essays submitted
12. **Mini Quiz Generator**
   - Questions from summary
13. **Feedback Modules**
   - Post-class input (student & teacher)
14. **Essay Token System**
   - Prepaid bundles for review requests

## ⏱️ Timeline (Estimates)
- Week 1–2: Auth, landing, basic roles
- Week 3–4: Zoom integration + subscriptions
- Week 5–6: Essay flows + admin v1
- Week 7–8: AI summaries, add-ons
- Week 9–10: Rescheduling, KPIs, QA

## 👥 Team Roles
- PM/Founder – weekly roadmap check-ins
- Frontend Dev – React components, dashboard logic
- Backend Dev – Directus config, Supabase queries
- QA – manual and automation pass
- AI Dev (optional) – Summary pipeline

## 🎯 Extras (Stretch)
- Notifications via email + Slack (admin alerts)
- PWA setup for mobile
- Gamification modules
- Parent dashboard (V3)

