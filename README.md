# Valuing Microlending Loans

---
## Technologies
This project leverages python 3.8.8 in jupyter lab 3.0.14 with the following packages:
- [Anaconda](https://www.anaconda.com/products/individual) - Pandas is included in Anaconda distribution and Conda package manager to manage Python environments.
- [Jupyter Lab](https://jupyter.org/) - web-based user interface designed for data analysis. It lets you write, run, and review the results in Python programs (all in a single integrated development environment (IDE).
---

## Part 1: Automate the Calculations
In this first part of the Challenge, you'll use loops and variables to automate the calculations for the loan portfolio summaries.

- Use the len() function to calculate the total number of loans in the list.
- Use the sum() function to calculate the total of all loans in the list.
- Using the sum of all loans and the total number of loans, calculate the average loan price.
- Print all calculations with descriptive messages.

## Part 2: Analyze Loan Data
Next, you'll use more detailed data for one of these loans to calculate present value, or fair price, of what this loan would be worth.

- Use get() on the dictionary of loan data to extract the future value and remaining months on the loan. Save these variables, named future_value and remaining_months, and then print each variable.
- Use the formula for present value to calculate the fair value of the loan. Use a minimum required return of 20% as the discount rate. You can find the the present value formula in the following image. More specifically, you'll want to use the monthly version of the present value formula:
Present Value = Future Value / (1+ Annual_Discount_Rate/12)**Months
- Now that you have the data you need, write a conditional statement (an if-else statement) to decide whether the present value represents the loan's fair value. If the present value of the loan is greater than or equal to the cost, then print a message that says that the loan is worth at least the cost to buy it. If the present value of the loan is less than the loan cost, then print a message that says that the loan is too expensive and not worth the price. If present value represents the loan's fair value (given the required minimum return of 20%), does it make sense to buy the loan at its current cost?

## Part 3: Perform Financial Calculations
Create a financial function that can be reused with new data values. To do this you’ll use the present value calculation. But you’ll place the calculation in a function so that the code can be reused in the future, if the company acquires new loans to consider.

- Define a new function to calculate present value. The function should meet the following criteria:
- Include parameters for future_value, remaining_months, and the annual_discount_rate.
- Return the present_value for the loan.
- Use the function to calculate the present value of the new loan. Use an annual_discount_rate of 0.2 for this new loan calculation.

## Part 4: Conditionally Filter Lists of Loans
 Loop through a series of loans that the company is considering and filter them to find the inexpensive ones.
 
 - Create a new, empty list named inexpensive_loans.
- Use a for loop to select each loan from a list of loans. Inside the for loop, write an if statement to determine whether the loan_price is less than or equal to 500.
- If the loan_price is 500 or less, append the loan to the inexpensive_loans list.
- Print the list of inexpensive loans.

## Part 5: Send a copy of your data as a spreadsheet or CSV for the company's business analysts.
In this final task of the Challenge, output your list of inexpensive loans to a CSV file. Use Python's csv library to create the csvwriter for this task.

- Use with open to open a new CSV file.
- Create a csvwriter using the csv library.
- Use the new csvwriter to write the header variable as the first row.
- Use a for loop to iterate through each loan in inexpensive_loans.
- Use the csvwriter to write the loan.values() to a row in the CSV file.

---
## Contributors
Presented by Bina Jariwala 

---
## License
none

---
