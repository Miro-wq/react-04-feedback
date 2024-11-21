# ✨ Feedback Widget, code refactoring using react hooks ✨

## 🛠 Tools used

[![My Skills](https://skillicons.dev/icons?i=html,css,js,react,npm,webpack,vscode)](https://skillicons.dev)

![Description](https://img.shields.io/badge/Description-purple?style=for-the-badge)
>This homework task focuses on building a simple feedback collection widget for Expresso Café, where customers can provide their opinions categorized as positive, neutral, or negative. Through this project, you will learn how to manage state in a React application, calculate and display statistics based on user input, and refactor code for better organization and reusability.

![Key Learning Objectives:](https://img.shields.io/badge/Key%20Learning%20Objectives-purple?style=for-the-badge)

- **State Management:** Gain experience in managing state within a React component, ensuring that the application dynamically updates based on user interactions.
- **Data Calculation:** Learn how to compute aggregate statistics, such as total feedback and the percentage of positive reviews, using helper methods.
- **Component-Based Architecture:** Practice structuring a React application by breaking down the user interface into reusable and maintainable components.
- **Conditional Rendering:** Implement conditional rendering to display content only when certain conditions are met, enhancing the user experience.

![Step 1](https://img.shields.io/badge/Step%201-purple?style=for-the-badge)

The application should display the number of reviews collected for each category. The application should not save statistics between different sessions (page refresh).

The state of the application should have the following structure; adding new properties is not allowed:

```js
state = {
  good: 0,
  neutral: 0,
  bad: 0
}
```

![Step 2](https://img.shields.io/badge/Step%202-purple?style=for-the-badge)

Extend the functionality of the application so that the interface displays more statistics about the collected reviews. Display the total number of reviews collected across all categories and the percentage of positive reviews.

To achieve this, create the helper methods `countTotalFeedback()` and `countPositiveFeedbackPercentage()`, which will calculate these values based on the state data (computed data).

![Step 3](https://img.shields.io/badge/Step%203-purple?style=for-the-badge)

Refactor the application. The application's state should remain in the root component `<App>`.

Move the statistics display into a separate component `<Statistics good={} neutral={} bad={} total={} positivePercentage={}>`.  
Move the button block into the `<FeedbackOptions options={} onLeaveFeedback={}>` component.  
Create the `<Section title="">` component, which will render a section with a title and children. Add the `<Statistics>` and `<FeedbackOptions>` components to this new component.

![Step 4](https://img.shields.io/badge/Step%204-purple?style=for-the-badge)

Extend the application’s functionality so that the statistics block is only rendered after at least one piece of feedback has been collected. Move the message about the absence of statistics into the `<Notification message="There is no feedback">` component.

