# 🧱 5-Day Drupal 10 Custom Module Development Training Plan

**🎯 Goal:** Build a complete, functional, and production-ready Drupal module from scratch by progressively adding components each day  
**Prerequisites:** Proficiency in PHP, OOP, YAML, and Drupal site building

---

## 🟦 Day 1: Module Scaffolding & Basic Routing

### Concepts:
- Module structure and `.info.yml` file  
- Routing (`.routing.yml`) and menu links (`.links.menu.yml`)  
- Controller basics and PSR-4 autoloading  
- Access control for routes  
- Using `t()`, render arrays, and simple output  
- Creating admin and user-facing pages

### Hands-On Tasks:
- Scaffold a new module (e.g., `custom_module`)  
- Add an admin page and frontend page  
- Add dynamic routing with parameters  
- Link pages through admin menu items

---

## 🟦 Day 2: Form API, Configuration & Services

### Concepts:
- Form API (`FormBase`, `ConfigFormBase`)  
- Building, validating, and submitting forms  
- Configuration API (editable config, default config)  
- Defining and injecting services (`*.services.yml`)  
- Using Messenger and Logger services  
- Third-party settings on existing entities

### Hands-On Tasks:
- Create a config form with settings  
- Save and retrieve config data  
- Build and inject a custom service  
- Use config and services inside a controller

---

## 🟦 Day 3: Hooks, Event Subscribers, Custom Block & Access Control

### Concepts:
- Common hooks (`hook_form_alter`, `hook_entity_presave`, etc.)  
- Creating Event Subscribers (`EventSubscriberInterface`)  
- Creating a custom block using `BlockBase`  
- Using permissions and `.permissions.yml`  
- Controlling access to routes and blocks  
- Adding AJAX to form elements

### Hands-On Tasks:
- Alter an existing form  
- Subscribe to and respond to entity lifecycle events  
- Build a configurable block  
- Protect routes with custom permissions  
- Add an AJAX-enabled button to a form

---

## 🟦 Day 4: Views Integration, Custom Fields, Widgets & Formatters

### Concepts:
- Views integration (`hook_views_data`, `hook_views_query_alter`)  
- Creating a custom field type (optional)  
- Custom field widgets and formatters  
- Exposing config/form data in Views  
- Theme hook implementation and template suggestions

### Hands-On Tasks:
- Add a custom field or formatter to your module  
- Make module data available in Views  
- Customize the output of a View using templates  
- Build a new formatter or widget and assign to existing fields

---

## 🟦 Day 5: Custom Entities, Schema, DB Tables, Updates & Cron

### Concepts:
- Creating a custom Content Entity (annotation-based)  
- Entity schema definition and CRUD form setup  
- Using `EntityListBuilder` and `EntityForm`  
- Creating custom DB tables (`hook_schema`)  
- Using `hook_install`, `hook_uninstall`, `hook_update_N()`  
- Writing cron tasks and batch operations  
- Packaging the module with `README.md`, versioning

### Hands-On Tasks:
- Create a simple custom content entity  
- Add admin UI for entity management  
- Define a custom table and use DB API  
- Add schema updates via `hook_update_N()`  
- Write a cron task to clean up data  
- Document and package the module for deployment

---

## ✅ Final Outcome

By the end of this course, learners will:
- Understand the entire module development workflow  
- Build a full-featured module from scratch  
- Implement configuration, services, events, blocks, Views, entities, and DB integration  
- Be able to structure and deploy maintainable modules across Drupal projects
