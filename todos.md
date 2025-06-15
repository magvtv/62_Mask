# TODOs.md - Mask Web App

## 🛠️ Core Development Tasks

### ✅ Authentication & Alias Setup

* [ ] Create signup/login system (email or device ID-based)
* [ ] Assign or allow creation of unique aliases (User123, BlueFox01, etc.)
* [ ] Prevent alias duplication

### ✅ Room Creation & Joining

* [ ] Build room creation interface
* [ ] Allow users to join via link or code
* [ ] Assign each message to a target alias within the room

### ✅ Message Posting

* [ ] Anonymous form for message submission
* [ ] Store message anonymously but tag with target alias
* [ ] Enforce cooldowns (e.g., max 3 messages/hour)

### ✅ Personal Feedback Dashboard

* [ ] Dashboard per user to show messages they’ve received
* [ ] Include tone indicators, tag clouds, and message history
* [ ] Allow filtering by sentiment

### ✅ Moderation Layer

* [ ] Integrate basic AI moderation (e.g., OpenAI Moderation API)
* [ ] Auto-flag messages with toxic language
* [ ] Admin interface for flag review

### ✅ Reporting System

* [ ] Flag/report message feature
* [ ] Shadowban repeat offenders
* [ ] Track karma/downvote ratio per user alias

### ✅ Public Profile Link

* [ ] Allow users to generate a shareable anonymous submission link (e.g., truthjar.com/ZRW42)
* [ ] All feedback via that link routes to dashboard

---

## 🎨 UX/UI Enhancements

### 🎭 Visual Identity

* [ ] Mask-themed design or dark/light switch mode
* [ ] Subtle transitions for feedback display

### 📊 Analytics

* [ ] Implement word cloud and tone graph
* [ ] Weekly recap view for each user

### ✨ Optional Gamification

* [ ] Karma points for submitting kind feedback
* [ ] Anonymous challenges ("Give 3 compliments this week")
* [ ] Weekly leaderboard for top aliases with most received feedback

---

## 🧪 Testing & Deployment

### 🧱 Backend

* [ ] Unit tests for message posting and retrieval
* [ ] Rate limit logic validation

### 🧪 Frontend

* [ ] Simulate multiple alias environments
* [ ] Accessibility testing

### 🚀 Deployment

* [ ] Set up Vercel / Netlify for frontend
* [ ] Deploy backend on Railway / Render / Heroku
* [ ] Use .env and GitHub secrets properly

---

## 📎 Future Features (Label as `enhancement` in Issues)

* [ ] Room-based sentiment analytics
* [ ] Voice notes (converted to text before submission)
* [ ] Auto-moderated feedback suggestions (GPT pre-filled tone options)
* [ ] Notification system for new messages received
* [ ] Mobile-first design with swipe interaction for feedback viewing
