# Loan Repayment Calculator

This is a simple, client-side web application for calculating loan repayment schedules with support for tracking actual monthly payments. It allows users to input loan details and specify exact payment amounts for any given month, providing a clear amortization table and summary.

## Features

* **Loan Details Input:** Easily enter the initial loan amount, start date, and yearly interest rate.

* **Agreed Monthly Payment:** Define your standard, agreed-upon monthly payment.

* **Actual Monthly Payments (Overrides):** Record the exact amount paid for specific months, overriding the agreed monthly payment for those periods. This is useful for tracking overpayments, underpayments, or payment holidays.

* **Dynamic Repayment Schedule:** Generates a detailed month-by-month table showing:

    * Starting Balance

    * Actual Payment Made

    * Interest Paid

    * Principal Paid

    * Ending Balance

* **Loan Summary:** Provides a quick overview including total interest paid, total principal paid, final repayment date, total payments made, and loan duration.

* **Euro Currency:** All monetary values are displayed in Euros (€).

* **State Persistence:** Your entered loan details and actual payment overrides are automatically saved in your browser's local storage, so they are remembered when you revisit the page.

## How to Use

1.  **Open the Calculator:** Open the `index.html` file in your web browser.

2.  **Enter Loan Details:**

    * **Loan Amount (€):** The total amount borrowed.

    * **Loan Start Date:** The date your loan begins.

    * **Yearly Interest Rate (%):** The annual interest rate of your loan.

    * **Agreed Monthly Payment (€):** Your regular, scheduled monthly payment.

3.  **Add Actual Monthly Payments (Overrides):**

    * Click the "Add Actual Payment" button.

    * For each entry, select the **Date** for which the payment was made and enter the **Actual Payment Made (€)**. This amount will override the "Agreed Monthly Payment" for that specific month in the calculation. You can enter `0` for a payment holiday.

    * Use the "Remove" button next to an entry to delete it.

4.  **Calculate:** Click the "Calculate Repayment Schedule" button to generate and view the detailed amortization table and loan summary.

## Deployment

This calculator is a static HTML, CSS, and JavaScript application, making it very easy and inexpensive to deploy online. Here are some recommended free options:

1.  **GitHub Pages:**

    * Host your code in a public GitHub repository.

    * Go to your repository's "Settings" -> "Pages".

    * Select your `main` (or `master`) branch and the `/ (root)` folder.

    * Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME/`.

    * Ideal for personal projects and simple static sites.

2.  **Netlify:**

    * Connect your GitHub repository to Netlify.

    * Netlify offers continuous deployment, automatically updating your site when you push changes to your repository.

    * Provides custom domains, SSL, and a generous free tier.

3.  **Vercel:**

    * Similar to Netlify, Vercel provides seamless Git integration for continuous deployment.

    * Known for its speed and developer experience, with a free Hobby plan suitable for this project.

## Local Development

To run this project locally:

1.  **Clone the repository** (if hosted on GitHub) or save the `index.html` file to your computer.

2.  **Open `index.html`** in your preferred web browser.

No server or build tools are required as all logic is handled client-side in the browser.

## Technologies Used

* **HTML5:** For the structure of the web page.

* **CSS3 (Tailwind CSS):** For styling and responsive design.

* **JavaScript:** For all the calculation logic, DOM manipulation, and local storage persistence.
