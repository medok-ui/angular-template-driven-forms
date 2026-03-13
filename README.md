# Angular Template-Driven Forms

> A hands-on project from the **Udemy course by Maximilian Schwarzmüller** — *Angular - The Complete Guide*.

---

## 📋 About This Project

This project demonstrates the use of **template-driven forms** in Angular — one of the two primary approaches to handling user input and form validation in Angular applications.

The main focus is a **Login Form** component that showcases how to bind form controls declaratively in the template using Angular's `FormsModule`, apply built-in validators, track control state, and persist user data between sessions via `localStorage`.

---

## 🚀 Features

- **Template-driven form setup** with `NgForm` and two-way binding via `ngModel`
- **Built-in validators** — `required`, `email`, `minlength` applied directly in HTML
- **Real-time validation feedback** — error messages shown only after the field is touched and dirty
- **Form submission handling** — reads values from `NgForm`, validates before processing, and resets after submission
- **LocalStorage persistence** — email field value is saved automatically with a `500ms` debounce and restored on the next visit using `afterNextRender`
- **Automatic subscription cleanup** via Angular's `DestroyRef`

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Angular (Standalone Components) | UI framework |
| `FormsModule` / `NgForm` | Template-driven form handling |
| `viewChild` | Access to the form reference |
| `afterNextRender` | Lifecycle hook for DOM-safe initialization |
| `DestroyRef` | Clean unsubscription on component destroy |
| RxJS `debounceTime` | Throttle localStorage writes |

---

## 🎓 Course Reference

This project is part of the course:

**[Angular - The Complete Guide (2024 Edition)](https://www.udemy.com/course/the-complete-guide-to-angular-2/)**
*by Maximilian Schwarzmüller on Udemy*

Section covered: **Forms — Template-Driven Approach**

---

## ▶️ Getting Started

```bash
# Install dependencies
npm install

# Start the development server
ng serve
```

Then open [http://localhost:4200](http://localhost:4200) in your browser.
