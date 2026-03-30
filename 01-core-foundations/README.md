# ⚛️ Core Foundations

A structured overview of fundamental React concepts. Click any topic to explore details.

---

## 📚 Concepts Index

| # | 📌 Topic |
|--|--------|
| 1 | [What is React?](#1-what-is-react) |
| 2 | [How React Works?](#2how-react-works) |
| 3 | [Benefits of React](#benefits-of-react) |
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


