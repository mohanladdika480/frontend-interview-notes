
### ⚛️ Core Foundations

A structured overview of fundamental React concepts. Click any topic to explore details.

---
<a name="table-of-contents"></a>
<details close>
<summary>📚 Table of Contents (Click to Expand/Collapse)</summary>

<br>

| # | 📌 Topic |
|--|--------|
| 1 | [What is React?](#1-what-is-react) |
| 2 | [How React Works?](#2-how-react-works) |
| 3 | [What are the advantages of React?](#3-what-are-the-advantages-of-react) |
| 4 | [What are the disadvantages of React?](#4-what-are-the-disadvantages-of-react) |
| 5 | [What are the major features of React?](#5-what-are-the-major-features-of-react)
| 6 | [What is Virtual DOM and how does it work?](#6-what-is-virtual-dom-and-how-does-it-work) |
| 8 | [What is Reconciliation (Diffing Algorithm)?](#7-what-is-reconciliation-diffing-algorithm) |
| 9 | [What are the phases of React rendering?](#8-what-are-the-phases-of-react-rendering) |
| 10 | [React Fiber](#react-fiber) |
| 11 | [Real DOM vs Virtual DOM vs Shadow DOM](#real-dom-vs-virtual-dom-vs-shadow-dom) |
| 12 | [Reflow & Repaint](#reflow--repaint) |

</details>

---

## 1. What is React?

React is an open-source JavaScript library used to build modern, interactive user interfaces, especially for single-page applications (SPAs).

It follows a declarative and component-based approach, allowing developers to create reusable UI components and manage complex interfaces efficiently.

React uses a Virtual DOM along with a reconciliation process to update only the parts of the real DOM that have changed, improving performance.

It also follows a one-way data flow, making applications more predictable, easier to debug, and easier to maintain.

It focuses only on the **view layer (UI)** of an application, making it a library rather than a full framework.

**[⬆ Back to Top](#table-of-contents)**

---

## 2. How React Works?

1. State or props change triggers a re-render.  
2. React creates a new Virtual DOM tree.  
3. It compares it with the previous Virtual DOM (reconciliation).  
4. Only the changed parts are updated in the real DOM.  
5. Updates are batched and optimized using techniques like concurrent rendering.  

**[⬆ Back to Top](#table-of-contents)**

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
  
**[⬆ Back to Top](#table-of-contents)**

---

## 4. What are the disadvantages of React?

- React is only a UI library, so features like routing, state management, and API handling are not built-in and require external libraries.
- It has a steep learning curve for beginners due to concepts like JSX, hooks, and state management.
- There are too many choices in the ecosystem (e.g., Redux, Context API, Zustand), which can lead to confusion in deciding the right approach.
- React has frequent updates and evolving patterns, requiring developers to continuously stay updated.
- SEO can be an issue in client-side rendered applications, but this can be addressed using server-side rendering frameworks like Next.js.

**[⬆ Back to Top](#table-of-contents)**

---

## 5. What are the major features of React?

### 🔵 Core Features

- **Component-Based Architecture**: Breaks UI into reusable, independent components, improving maintainability and scalability  
- **JSX (JavaScript XML)**: Allows writing HTML-like syntax inside JavaScript, making UI code more readable  
- **Virtual DOM & Reconciliation**: Uses a virtual representation of the DOM and updates only changed parts efficiently  
- **Declarative UI**: Developers describe how UI should look, and React handles updates  
- **One-Way Data Flow**:Data flows from parent to child, making state predictable and easier to debug  
- **Hooks**: Enable state and lifecycle features in functional components (e.g., useState, useEffect)  


### 🟠 Advanced Features

- **Context API**: Avoids prop drilling by sharing data globally  
- **Error Boundaries**: Handle runtime errors in UI without crashing the entire app  
- **Concurrent Rendering**: Improves responsiveness by prioritizing important updates  
- **React Server Components**: Reduce client-side JavaScript and improve performance  
- **Suspense**: Handles loading states for async operations (like data fetching or lazy loading)

**[⬆ Back to Top](#table-of-contents)**

---

## 6. What is Virtual DOM and how does it work?

Virtual DOM is a lightweight JavaScript representation of the real DOM. React uses it to efficiently track changes in the UI and update only the necessary parts of the real DOM instead of re-rendering the entire page.

### Working:

1. When a component is initially rendered, React creates a Virtual DOM tree.  
2. When state or props change, React creates a new Virtual DOM.  
3. React compares the new Virtual DOM with the previous one using reconciliation (diffing algorithm).  
4. React identifies the differences between the two Virtual DOM trees.  
5. Only the changed elements are updated in the real DOM.  

**[⬆ Back to Top](#table-of-contents)**

---

## 7. What is Reconciliation (Diffing Algorithm)?

Reconciliation is the process by which React compares the previous Virtual DOM with the new Virtual DOM to identify differences and efficiently update only the changed parts in the real DOM.

### Heuristic Rules

React uses heuristics like element type and keys to optimize the diffing process and reduce complexity from O(n³) to O(n).

1. **Different Element Types**  
   Old: `<div>` → New: `<span>`  
   → React replaces the entire subtree  

2. **Same Element Type**  
   `<div>` → `<div>`  
   → React updates only the changed attributes  

3. **Lists with Keys 🔥**  
   Keys help React identify:
   - Which items changed  
   - Which items moved  
   - Which items were added or removed  

   → Without keys, React may cause poor performance and UI bugs  

**[⬆ Back to Top](#table-of-contents)**

---

## 8. What are the phases of React rendering?

