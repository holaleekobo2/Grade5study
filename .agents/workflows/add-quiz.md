---
description: How to add a new quiz to the website
---

Follow these steps to add a new quiz to the Grade5study website:

1.  **Create a new HTML file**:
    Copy `template_quiz.html` to a new filename (e.g., `science_unit2_quiz1.html`).
    ```bash
    cp template_quiz.html science_unit2_quiz1.html
    ```

2.  **Update Quiz Metadata**:
    Open the new file and update the following:
    - `<title>`: The title of the page.
    - `<h1>`: The heading of the quiz.
    - `STORAGE_KEY`: A unique string for `localStorage` (e.g., `science_unit2_quiz1_results`).
    - `quizData`: The array containing your questions, options, and the index of the correct answer (0-indexed).

3.  **Link the Quiz**:
    Open the relevant subject page (e.g., `science.html`) and add a link to your new quiz in the appropriate section.
    Example:
    ```html
    <li>
        <a href="science_unit2_quiz1.html" class="quiz-link">
            📝 測驗 1：新單元標題
        </a>
    </li>
    ```

4.  **Verify**:
    Open the website in your browser (via the local preview server) and test the new quiz to ensure it works as expected.
