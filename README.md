This Java application assists users in planning their personal budget by calculating various expenses and loan repayments.
It allows users to input their gross monthly income, estimated monthly tax, and costs for different expense categories such as groceries, utilities,
travel, phone, and other expenses. Users can choose between renting accommodation or buying a property. For renting, users input their monthly rent amount,
while for buying, they input the property price, deposit, interest rate, and repayment period to calculate monthly loan repayments.
The application calculates the interest rate on a property and the monthly loan repayment amount using methods from the LoanCalculator superclass.
It also checks if the loan repayment exceeds the user’s gross monthly income and provides feedback on the likelihood of loan approval.
The program is structured with a LoanCalculator class that includes methods for calculating interest rates and loan repayments, and a PersonalBudgetPlanning class that extends LoanCalculator
and contains the main method for user interaction. To use the program, clone the repository, navigate to the project directory, compile the program using javac PersonalBudgetPlanning.
java, and run it with java PersonalBudgetPlanning. Ensure you have the Java Development Kit (JDK) installed to compile and run the program.


Program Start:

The application starts in the main method of the BudgetPlanner class.
The first step is to create a Scanner object to handle user input from the console.
User Input for Income:

The user is prompted to enter their gross monthly income. This value is stored in the grossIncome variable.
Estimated Tax Input:

Next, the user is asked to enter the estimated monthly tax deducted, which is also captured for later calculations.
Monthly Expenditures Input:

The user is prompted to enter their estimated monthly expenditures across various categories:
Groceries
Water and lights
Travel costs
Cell phone and telephone
Other expenses
Each input is stored in separate variables and can be summed later to determine total monthly expenses.
Accommodation Decision:

The user is asked whether they would like to rent or buy a property. The input is case-insensitive.
If the user chooses to rent, they are prompted to enter the monthly rental amount. This is added to the list of expenses.
If they choose to buy a property, they are prompted to enter:
Purchase price of the property
Total deposit
Interest rate (as a percentage)
Number of months to repay the loan (between 240 and 360 months)
A HomeLoan object is created using the entered data, which calculates the monthly repayment amount using a method inside the HomeLoan class.
Loan Approval Check:

If the calculated monthly repayment for the home loan exceeds one-third of the user's gross income, a warning message is displayed, indicating that loan approval is unlikely.
Vehicle Purchase Option:

The user is then asked if they wish to buy a vehicle. If they respond with "yes", they are prompted to enter:
Vehicle purchase price
Total deposit
Interest rate (percentage)
Estimated insurance premium
A VehicleLoan object is created, which combines the insurance and loan repayment costs into one expense that is added to the expenses list.
Calculate Available Monthly Money:

The application calculates the available monthly money by subtracting total expenses (including tax and loan repayments) from the gross income.
This value is displayed to the user.
Expense Limit Warning:

If the total expenses (including loan repayments) exceed 75% of the gross income, the user receives a warning about their spending.
Display Expenses:

The program sorts all recorded expenses in descending order based on their amount and prints them to the console, allowing the user to see where their money is going.
Code Execution Steps
Here’s a concise step-by-step breakdown of the execution:

Initialization: The program initializes necessary variables and collections to hold user input data.
Input Handling: It uses a loop of prompts to gather user input, validating as necessary (though basic in this implementation).
Calculations: It calculates loan repayments and available money based on user inputs.
Conditional Logic: It uses conditions to provide warnings based on the user's financial data (e.g., loan approval likelihood and expense limits).
Output: Finally, it displays results and sorted expenses to the user.
Example Walkthrough
User inputs a gross monthly income of 5000.
Estimated tax deducted is 1000.
Monthly expenditures:
Groceries: 600
Water and lights: 200
Travel costs: 150
Cell phone and telephone: 100
Other expenses: 200
User chooses to rent and inputs a rental amount of 1200.
User is asked about buying a vehicle and inputs vehicle details, leading to a vehicle loan being added to the expenses.
The application calculates total expenses, available money, and checks for conditions like loan approval likelihood and total expenses exceeding 75% of the income.
All expenses are displayed in descending order, allowing the user to review their financial situation effectively.
Conclusion
This application provides a clear structure for managing personal finances, allowing users to visualize their income and expenses. It encourages budgeting awareness
and offers valuable insights into potential financial burdens, such as loan repayments.

