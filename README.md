# Assaignment 5 Requirement 6  Q&A

### What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll? 
**Difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll :**
- **getElementById('id')**: Selects a single element by its unique ID.
- **getElementsByClassName('class')**: Selects a live HTMLCollection of all elements with the given class name.
- **querySelector('css-selector')**: Selects the first element that matches the given CSS selector.
- **querySelectorAll('css-selector')**: Selects a static NodeList of all elements that match the CSS selector.

### How do you create and insert a new element into the DOM?
**To create and insert a new element into the dom those way:**
1.  **Create** the element: `const newEl = document.createElement('div');`
2.  **Insert** it into the DOM: `parentElement.appendChild(newEl);` (or `insertBefore`, `append`, `prepend`)

### What is Event Bubbling and how does it work?
Event Bubbling is an event that begins at the target element and moves upward through all of its ancestor elements in the DOM hierarchy.

### What is Event Delegation in JavaScript? Why is it useful?
Event Delegation is when we add a single event listener to a single parent, and that listener is responsible for handling any events for child elements of that parent. Event Delegation is effective for performance reasons (fewer listeners), and to avoid problems with dynamically added elements.

### What is the difference between preventDefault() and stopPropagation()?
- **preventDefault()**: Cancels the default behaviour of the browser concerning the event that just took place (for instance: when using form submit or navigating to a link).
- **stopPropagation()**: Stops the event from bubbling up or capturing down the DOM tree thus preventing other listeners from learning about the event.