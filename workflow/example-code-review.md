# Example Code Review: AI-Assisted Development
## More complex code review will be included in the final draft
## Overview
This section is deticated to deomnstrating how AI-generated code can look correct but still contain problems that developers are responsible for fixing. 

The following example containts a simple React component that my teamates from CMPSC 156 will be familiar with.

This is just a hypothetical example and not part of any specific code base
## 1. AI-Generated Code

Example prompt: create a react component that displays a course's information. 

AI output: 

```jsx
function CourseInfo({ course }) {
  return (
    <div>
      <h2>{course.title}</h2>
      <p>{course.description}</p>
    </div>
  );
}
```

A quick glance at this output could lead someone to believe that this is a correct implementation. 

However, there is a problem that might not immediately be noticed.

## 2. Identifying the Problem

The bug in this implementation is a lack of error handling. If the component recieves a course with invalid information such as 'null or 'undefined' then the program could throw an error or create unexpected behavior. 


## 3. Human Review and Correction

After reviewing the code, the developer could modify the component to handle missing information.

```jsx
function CourseInfo({ course }) {
  if (!course) {
    return <p>Course information unavailable.</p>;
  }

  return (
    <div>
      <h2>{course.title}</h2>
      <p>{course.description}</p>
    </div>
  );
}
```

This version handles the case where no course object is provided. However, the developer is still responsible for considering other possible bugs or issues with the generated output. 


## 4. Applying the Checklist

Using my [Code Review Checklist](../guidelines/code-review-checklist.md), the developer should be able to answer the following questions:

- Do I understand how this implementation works?
- Does the code handle unexpected inputs?
- Have I tested the component with valid and missing course data?
- Could another developer understand and maintain this code?

## Final Takeaway
Overall, this is a simple example of how AI can sometimes miss the small details that are important in software engineering. The original code could have passed all tests and checks if tests missed proper edge cases. This is a great example of why human review should still be a central part of the development cycle. 


My intention is not to suggest that AI-generated code is always incorrect but to show why developers should understand and verify their implementations instead of relying entirely on automated testing.