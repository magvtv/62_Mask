# 62_Mask - Anonymous Truth Web App

## Overview

"A man is least himself when he talks in his own person. Give him a mask, and he will tell you the truth." — Oscar Wilde.

**Mask** is a web application inspired by the social psychology of anonymous confessions. It enables users to anonymously submit and receive messages within a structured group or room environment. The app is structured around the idea that individuals are more likely to express honest thoughts when their identity is concealed. It aims to combine the anonymity of apps like NGL and Sarahah with a new twist: a personal dashboard of what others have anonymously said about you.

---

## Features

### 1. **Anonymous Message Rooms**

* Users can join public or closed rooms (e.g., "3rd Year Computer Science" or "Dorm Alpha").
* Messages are submitted anonymously by anyone in the room.
* Each message must be tagged to a user alias (e.g., `ZRW42`) but not the author.
* There is no way to trace who submitted a message.

### 2. **Alias System (Target Identity)**

* Every user gets a unique **alias** (e.g., `UserX42` or custom handles like `theMaskedOne`).
* Aliases can be shared with others to receive feedback anonymously.
* A user can only view messages where they are the **target alias**.
* Should they be able to update their aliases?

### 3. **Personal Feedback Dashboard**

* Logged-in users see an exclusive dashboard with:

  * All messages sent about them.
  * No visibility into others' feedback.
  * Visual analytics like tone clouds, word trends, or timeline breakdowns.

### 4. **AI-Powered Moderation Engine**

* All messages pass through a basic **toxicity filter**.
* Optional: Use NLP tone analysis to auto-label the tone (supportive, sarcastic, flirty, etc.).
* Report and flag system to penalize misuse.

### 5. **Gamified Prompts & Leaderboards** *(Optional)*

* Weekly anonymous challenges: “Say something kind to 3 people.”
* Confession-based games: “Can you guess who this is about?”
* Karma system for upvotes/downvotes to highlight meaningful content.

### 6. **Room Management (Admin or Trusted Roles)**

* Room creators get moderation powers (mute, remove, shadowban users).
* Room activity scores to promote healthy interactions.

### 7. **Privacy by Design**

* No IP or metadata exposed to clients.
* Timestamp masking to reduce identity deduction.
* Messages are ephemeral (optional auto-delete after 30 days).

### 8. **Shareable Profile Pages**

* Users can share a public-facing page (e.g., `truthjar.com/ZRW42`) where others can submit thoughts anonymously.
* Feedback here still routes to private dashboard.

---

## Tech Stack Suggestion

### Frontend

* **Vue.js** or **React**
* TailwindCSS for clean UI

### Backend

* Node.js + Express or Django REST Framework
* Socket.IO (optional for real-time)

### Database

* MongoDB or Firebase

### NLP & AI Tools

* OpenAI Moderation API or Perspective API for toxicity filtering
* Basic tone classifier using HuggingFace transformers or similar

---

## Repository Usage

### Issues Section

* Use `feature:` label to propose new features
* Use `bug:` label for functional problems
* Use `enhancement:` for UI/UX or logic improvements
* Use `security:` for anonymity or abuse vulnerabilities

---

## License

MIT

