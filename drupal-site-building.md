# 🏗️ Drupal 10 Site Building Training Plan (Week 1)

**🎯 Use Case:** Build a fully functional “Event Management” site using Drupal Admin UI — no custom code  
**👥 Audience:** Beginner to Intermediate Drupal users  
**🛠 Tools:** Drupal Core, Contributed Modules (Pathauto, Webform, Media, Layout Builder, Views, etc.)

---

## 🟦 Day 1: Drupal Fundamentals & Content Modeling

### 🎯 Objectives:
- Understand Drupal's architecture and site building philosophy
- Set up local development environment
- Create content types and fields for event management

### 📘 Key Concepts:
- Nodes, Entities, Fields, Bundles
- Admin UI overview
- Configuration vs content
- Revisions and Publishing

### 🛠 Hands-On:
- Install Drupal 10
- Configure site settings (timezone, language)
- Create “Event” content type with fields:
  - Title (default)
  - Event Date (Date)
  - Event Time (Time)
  - Venue (Text)
  - Event Status (List: Upcoming, Ongoing, Cancelled)
  - Description (Text area with CKEditor)
  - Event Photos (Media → Image, multiple)
- Add sample event content

---

## 🟦 Day 2: Categorization, Navigation, and URL Management

### 🎯 Objectives:
- Categorize events using taxonomy
- Create intuitive menus
- Set up URL aliasing with Pathauto

### 📘 Key Concepts:
- Taxonomy Vocabularies & Terms
- Menus and Menu Links
- Pathauto for clean URLs

### 🛠 Hands-On:
- Create “Event Type” taxonomy: Conference, Webinar, Workshop
- Add term reference to Event content type
- Create custom main menu: Home, Events, Submit Event, About
- Install & configure Pathauto:
  - Pattern: `/events/[node:title]`

---

## 🟦 Day 3: Media, Image Styles & Layout Builder

### 🎯 Objectives:
- Reuse images with Media Library
- Create image styles for consistent display
- Customize layouts with Layout Builder

### 📘 Key Concepts:
- Media module, Media Library
- Image Styles: Crop, Resize, Scale
- Display Modes: Teaser, Full
- Layout Builder UI

### 🛠 Hands-On:
- Enable Media module & Media Library
- Upload and reuse Event Photos
- Create and apply Image Styles:
  - Thumbnail (200x200, crop)
  - Event Banner (900x300, crop & scale)
  - Teaser Image (400x200)
- Apply styles in Display Modes
- Enable Layout Builder for Event content type
- Customize full view layout: add images, metadata, term blocks

---

## 🟦 Day 4: Views - Dynamic Event Listings

### 🎯 Objectives:
- Build dynamic event listings with Views
- Create block and page displays
- Add filters and sorting to listings

### 📘 Key Concepts:
- Views (Page vs Block)
- Filters, Exposed Filters, Sort Criteria
- Relationships, Display Formats
- Pagination and RSS feeds

### 🛠 Hands-On:
- Create View: "Browse Events"
  - Path: `/events`
  - Display fields: Image, Title, Date, Type
  - Sort by Event Date
  - Exposed Filters: Event Type, Date
  - Add pagination

- Create Block View: "Upcoming Events"
  - Filter: Event Date >= today
  - Sort: Event Date ascending
  - Limit: 5 results
  - Display: Title, Date
  - Place in sidebar using block layout

- Enable RSS feed for events listing

---

## 🟦 Day 5: Permissions, Webforms & SEO Prep

### 🎯 Objectives:
- Create user roles and assign permissions
- Create forms with Webform module
- Improve SEO readiness

### 📘 Key Concepts:
- Roles and Permissions
- Webform basics
- Meta Tags, Redirects, Sitemap
- Content Moderation (optional)

### 🛠 Hands-On:
- Create Roles: Event Viewer, Event Editor, Event Manager
- Assign permissions accordingly
- Install & configure Webform:
  - Form: “Submit an Event”
  - Fields: Title, Description, Email, Event Date
  - CAPTCHA & email notifications

- Install and configure SEO modules:
  - Meta Tags
  - Redirect
  - Simple XML Sitemap

- Final Review:
  - Responsive layout test
  - Navigation usability
  - SEO checks
  - Content entry & user workflow

---

## ✅ Outcome:
- A fully functional Event Management site
- Mastery of site building tools: Content types, Media, Views, Layout Builder
- Structured taxonomy and menus
- User-submitted content and role-based workflows
