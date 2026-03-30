# ⚛️ Core Foundations

A structured overview of fundamental React concepts. Click any topic to explore details.

---

## 📚 Concepts Index

| # | 📌 Topic |
|--|--------|
| 1 | [What is React?](#1-what-is-react) |
| 2 | [How React Works?](#2-how-react-works) |
| 3 | [What are the advantages of React?](#3-what-are-the-advantages-of-react) |
| 4 | [Disadvantages of React](#disadvantages-of-react) |
| 5 | [React vs Angular vs Vue](#react-vs-angular-vs-vue) |
| 6 | [When to Choose What](#when-to-choose-what) |
| 7 | [Virtual DOM](#virtual-dom) |
| 8 | [How does Virtual DOM Works](#how-virtual-dom-works) |
| 9 | [Reconciliation (Diffing Algorithm)](#reconciliation-diffing-algorithm) |
| 10 | [Component Rendering Process](#component-rendering-process) |
| 11 | [React Fiber](#react-fiber) |
| 12 | [Real DOM vs Virtual DOM vs Shadow DOM](#real-dom-vs-virtual-dom-vs-shadow-dom) |
| 13 | [Reflow & Repaint](#reflow--repaint) |
| 14 | [Library vs Framework](#library-vs-framework) |
| 15 | [SPA vs MPA](#spa-vs-mpa) |
| 16 | [CSR vs SSR vs SSG](#csr-vs-ssr-vs-ssg) |
| 17 | [Hydration](#hydration) |

---

## 1. What is React?

React is an open-source JavaScript library used to build modern, interactive user interfaces, especially for single-page applications (SPAs).

It follows a declarative and component-based approach, allowing developers to create reusable UI components and manage complex interfaces efficiently.

React uses a Virtual DOM along with a reconciliation process to update only the parts of the real DOM that have changed, improving performance.

It also follows a one-way data flow, making applications more predictable, easier to debug, and easier to maintain.

It focuses only on the **view layer (UI)** of an application, making it a library rather than a full framework.

---

## 2. How React Works?

- When a component is initially rendered, React creates a Virtual DOM (V-DOM), which is a lightweight copy of the real DOM.  

- When state or props change, React creates a new Virtual DOM.  

- React compares the new Virtual DOM with the previous one to identify the changes. This process is called Reconciliation (Diffing Algorithm).  

- Only the changed parts are updated in the real DOM instead of re-rendering the entire UI.

--- 

## 3. What are the advantages of React?

1. **Component-Based Architecture**  
   - Breaking the UI into independent, reusable components, where each component manages its own logic and UI.
   - This improves code reusability, maintainability, and makes large applications easier to scale and manage.

2. **High Performance (Virtual DOM)**  
   - Updates only changed parts of the UI  
   - Faster than direct DOM manipulation  

3. **Declarative Approach**  
   - React follows a declarative approach, where developers define how the UI should look based on the state, and React handles updating the DOM efficiently.

4. **Reusable Components**  
   - Write once, use multiple times  
   - Reduces code duplication  

5. **One-Way Data Flow**  
   - Data flows from parent to child components, making the application more predictable and easier to debug.

6. **Strong Ecosystem & Community**  
   - React has a strong ecosystem with a wide range of libraries and tools for routing, state management, and testing, supported by a large community.

7. **Scalable for Large Applications**  
   - React supports scalability by enabling modular architecture and efficient state management, making it suitable for large-scale applications.

---
