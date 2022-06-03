ST10084788 POE PART 2 ReadMe
Project Title: PROG6221 POE Part 2 – Budget Planner Application

Motivation: This project was created as part of my POE for Programming 2A module. 

Build status: The budget application has been fully completed.

Introduction:
The PROG6221 POE comprises of three parts, so far, I have completed the second part of the POE. 
In part 1 of the PROG6221 POE, we have been tasked to develop a budget planner application. The budget planner application that I have developed will require the user’s salary, tax amount, and expenses - the application will then calculate the user's monthly available amount after all expense deductions. The budget planner application starts off by asking users to input their gross salary and estimated tax amount. It then proceeds to ask the user to enter the estimated amounts that they would spend on the basic expenses such as groceries, lights and water, travel costs, and phone billing costs. The user also has an option to select if they would like to rent an accommodation or buy a property. If the user selects the rent option, they would then be asked to input the rental amount. If the user selects the option to buy a property, they would be directed to a home loan calculator, which would then ask the user to input the necessary details, and then calculate the monthly home loan repayment amount- the program would also notify the user if the home loan were unlikely to be approved. 
In part 2 of the PROG6221 POE, I have added more features to the budget planner application, as well as improve the overall design and functionality of the project. The added features now include the option for the user to purchase a vehicle, if the user chooses to buy a vehicle, the app will calculate the monthly instalments that the user will pay towards the vehicle. The vehicle monthly instalment and insurance premium are then added to the user’s expenses. The program also uses a delegate notify the user if their expenses have exceeded over 75% of their salary. Another added feature, the expenses are now displayed in decreasing order.





Input And Output For Budget Planner Application:

The user would have to input the following data:
•	Gross salary before deductions
•	Estimated tax amount 
•	Estimated expenditure on basic expenses (groceries, lights and water, travel costs, phone billing)
•	Name and amount for any additional expenses
•	If the user chooses to rent a property, they will be required to provide the rental amount 
•	If the user chooses to buy a property, they will be required to provide the purchase price of the property, the total deposit paid, the interest rate, and months to repay home loan.
•	If the user chooses to buy a vehicle, they will be required to provide the model make and number, purchase price, total deposit paid, interest rate, and insurance premium 

The program will then output the following data:
•	Salary after tax deduction
•	Expenditure of all expenses in descending order 
•	Rental fee
•	Calculated monthly home loan repayment fee
•	Vehicle information such as make and model number
•	Calculated monthly vehicle repayment fee
•	The available balance after all deductions have been made

Features of the program:
•	The program will store all your basic expenses and any additional expenses
•	The program calculates the home loan monthly repayment amount
•	The program calculates your monthly vehicle repayment amount
•	The program calculates your monthly available amount after all expense deductions
•	The program will notify you if your expenses have exceeded over 75% of your salary
•	The program list all the expenses in descending order



The Budget Planner Application Was Developed Using The Following Software:
•	Visual Studio 2022 Community Version
•	Console app (.NET Framework 4.7.2.)
•	Microsoft Windows 11 OS
•	Git
•	GitHub
•	Word
(No additional plug-ins were used)

The Budget Planner Application Was Developed Using The Following Hardware:
•	Processor: 11th Gen Intel® Core™ i5-11400H @2.70GHZ, 2688 Mhz, 6 Core(s), 12 Logical Processor
•	RAM: 8GB
•	Disk Space Available: 319 GB

Software And Hardware requirements to run the program:
•	Windows 7 or higher
•	Visual Studio 2019 or higher
•	Requires a 2.6 GHz or faster processor. Quad core or better recommended.
•	Requires 4 GB of RAM or higher for load generation.
•	Requires 10 GB of hard disk space.

Basic structure of the program:
The program consists of five classes:
•	Program class (main class)
•	PopulateArrays class
•	Expense class
•	Rental class
•	HomeLoan class
•	Vehicle Class




The program class is the main class that consists of the following methods:
•	DisplayMenu(): Displays main menu to user
•	BudgetPlanner(): Asks user to input expense amount for all basic expenses
•	ValidateData(): Asks user to enter value again
•	MoreExpensesOrVehicle(): Asks user if they would want to purchase a vehicle or add any additional expenses
•	ExtraExpenses(): Adds additional expenses to arraylist
•	Accommodation()
•	BuyProperty()
•	RentAccommodation()
•	ExitApplication()
•	LoadingSummary()
•	ShowSpinner()
•	WelcomeAnimation()
•	EndOfProgram()
•	carChoice()
•	EnterVehicleDetails()
•	NotifyUser
•	DelegateMethod()
The populateArrays class holds the arraylists and the following methods:
•	SumArr()
•	SortArray()
The Expense class is an abstract class that contains an abstract method called CalculateMonthly
The Rental, Home Loan, and Vehicle class extend the Expense class.

Change Log
•	Delegate added
•	carChoice method created
•	EnterVehicleDetails method created
•	NotifyUser method added
•	DelegateMethod
•	In part one, I had two abstract methods in the Expense class- I have now removed the BudgetReport method as an abstract method. There is currently only one abstract method which is the CalculateMonthly method


Frequently Asked Question (FAQ):
1. Why won't the program allow me to enter an expenditure value with a full stop (Example: 10.3)?
Answer: Throughout the program, you are only allowed to enter a decimal value with a comma (Example: 10,3). The use of full stops in a decimal value does not work for the program. 

2. For my tax amount, should I enter it as the tax percentage or the actual tax amount that is deducted from my salary?
Answer: With regards to the tax amount, please enter the estimated the tax amount that is deducted from your salary, do not enter the tax percentage- the program works with the actual tax amount. 

3. How many additional expenses can I add?
Answer: You may add as many additional expenses as you would like to. 

4. For the monthly home loan repayment calculator, is there only two possible options for the months?
Answer: Yes, you will either select 240 months or 360 months. 

5. What does the monthly available amount mean? 
Answer: The monthly available amount is your remaining balance of your salary after all your expenses deductions (tax amount, basic expenses, additional expenses, rent/monthly home loan repayment and/or monthly car instalment fee).

6. Does the program only calculate one budget report every time it is executed?
Answer: No, after you have completed a budget report, you will be presented with the option to return to the main menu or exit the application, you can then select the main menu option and work on a different budget plan




How To Compile And Run Program:
Method 1:
•	Have Visual Studio installed
•	Open the source code folder that is in the project folder, and double click on the 'Visual Studio Solution File'
•	The solution file will then open in the visual studio application
•	Once it has loaded, select the 'Start' button located on the top panel of the application
•	The program will begin to compile and run

Method 2:
•	Once you have opened the file in visual studio
•	Press Ctrl+F5
•	Select Debug 
•	Start without debugging

Method 3:
•	Open the project folder
•	Navigate to the source code folder
•	Locate and the bin folder
•	Select the debug folder
•	Double on the ‘Application’ file


Difficulties I Have Encountered Whilst Developing The Budget Planner Application:
The first distinct problem that I had encountered was storing the expenses into either a normal array or an arraylist. I decided to then use an arraylist because the size of an arraylist is expandable. I thought that the Arraylist would be ideal for the budget planner application because the user does have a choice to enter more than one additional expense. If I had used an array, then the user would not be able to add multiple additional expenses as the sized of the array needs to be predefined.
The second problem was determining whether the user had decided to purchase a vehicle and then from that calculate the monthly available amount. The solution that I have used to fix this problem was to introduce a carOption variable to the program. This variable is of integer type. If the user selects the option to purchase a vehicle, the car option is automatically set to one. If they do not choose to purchase a vehicle, the carOption variable is set to zero. From there I sent the carOption variable to CalculateAvailableAmount method. 
The third major problem that I encountered was displaying the arraylists in descending order along with the correct expense name next to it. A solution that I used to solve this problem, was to convert the arraylists to arrays and then sort the arrays in ascending order as parallel arrays. I then displayed the items in the array by using a loop. 


Code Attribution
1. dotnet-bot (n.d.). Double.TryParse Method (System). [online] docs.microsoft.com. Available at: https://docs.microsoft.com/en-us/dotnet/api/system.double.tryparse?view=net-6.0 [Accessed 13 May 2022].
2. dotnet-bot (n.d.). Timer Class (System.Timers). [online] docs.microsoft.com. Available at: https://docs.microsoft.com/en-us/dotnet/api/system.timers.timer?redirectedfrom=MSDN&view=net-6.0 [Accessed 13 May 2022].
3. www.c-sharpcorner.com. (n.d.). ArrayList in C#. [online] Available at: https://www.c-sharpcorner.com/UploadFile/3d39b4/arraylist-in-C-Sharp/ [Accessed 13 May 2022].
4. www.informit.com. (n.d.). Basic Error Handling with Exceptions | C# Methods and Parameters | InformIT. [online] Available at: https://www.informit.com/articles/article.aspx?p=2923212&seqNum=9.
5. GeeksforGeeks. (2018a). C# | Delegates. [online] Available at: https://www.geeksforgeeks.org/c-sharp-delegates/#:~:text=Delegate%20type%20can%20be%20declared [Accessed 3 Jun. 2022].
6. GeeksforGeeks. (2018b). C# | How to convert an ArrayList to Array. [online] Available at: https://www.geeksforgeeks.org/c-sharp-how-to-convert-an-arraylist-to-array/ [Accessed 3 Jun. 2022].
7. Stack Overflow. (n.d.). c# - Sorting an array related to another array. [online] Available at: https://stackoverflow.com/questions/1964234/sorting-an-array-related-to-another-array.








What changes have been made from the lecturer’s feedback?
•	Comments have been improved. The comments are now more specific and go into more detail about the code. More comments have been added to the program as well. Comments that were irrelevant and held no meaning have been removed.
•	The exit loop issues have been fixed, in part one of the POE, I had called methods while still in the while loop, I have now corrected that so that the methods are now called after the loop has been exited- in that way the program does not run in a nested loop- this saves on the memory consumed by the program.
•	Minor errors such as spelling and missing words have been corrected
•	I have changed my display methods (display methods for the budget report) so that they can be displayed in a way that is easier for the user to read and comprehend- to do this, I made it more explicit as what the exact expense costs were.
•	The read me file now has more information about the program- it now includes the hardware specifications to run the program, and what software was used to create the program. 
•	Warnings have been improved- all warnings have now been highlighted in a distinct colour.


Developer Information
Developer Name: Shivani Naidu
Student email: ST10084788@vcconnect.edu.za
Contact number: 0743432766

GitHub Link
I have create a main branch, and a second branch called secondlink. 
The main branch has all the files for part one of the POE and the secondlink branch has all the files for the part two of the POE.
Link to GitHub main branch: https://github.com/niniiibae/ST10084788-PROG6221-POE-Part-1.git
Link to GitHub secondlink branch: https://github.com/niniiibae/ST10084788-PROG6221-POE-Part-1/tree/secondlink/ST10084788_PROG6221_POE_PART_2
Link to Kanban board for Part 1: https://github.com/niniiibae/ST10084788-PROG6221-POE-Part-1/projects/1

Link to Kanban board for part 2: https://github.com/niniiibae/ST10084788-PROG6221-POE-Part-1/projects/2?add_cards_query=is%3Aopen




