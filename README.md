# Financial_Planning
Week 5 Homework Financial Planning Analysis Tool 

The directory Financial_Planning contains the MCForecastTools file used and the final draft of my code the financial-planner file.
There is no .env or .gitignore as my environment variables are stored in my system users. 

The Following is the approach and plan I followed as stated in the financial-planner file:

- I will be developing a prototype application to demo in the next credit union assembly. (financial analysis tools)

- The first will be a personal finance planner that will allow users to visualize their savings composed by investments
in shares and cryptocurrencies to assess if they have enough money as an emergency fund.

- The second tool will be a retirement planning tool that will use the Alpaca API to fetch historical closing prices for 
a retirement portfolio composed of stocks and bonds, then will run Monte Carlo simulations to project the portfolio performance at 30 years. 
then will then use the Monte Carlo data to calculate the expected portfolio returns given a specific initial investment amount.

- The optional task will be running Monte Carlo simulations to project the portfolio performance at 5 and 10 years to see what is required for early retirement.

-- The Process:
-- Part 1 Personal Finance Planner
1. Set initial imports for whole code
2. Load environment variables 
3. Get URL from alternative api for BTC and ETH, and set variables with holdings of those coins
4. Request.get from both URL and single out the price of both coins into seperate variables for current price
5. Then will print the total balance of our holdings
6. Next need to collect investment data with Alpaca api
7. First will set variables for current amount of shares in both
8. Will get API keys and check if they loaded correctly 
9. Create an api object 
10. Then will set all variables for the alpaca.get_barset then run and print it 
11. Put the latest close price of both into sperate variables and print to view
12. Next is savings health analysis, will create a new dataframe with both the crypto and share closing prices combined
13. Will plot in pie chart to see the weights/risk of the portfolio
14. Then will make an if statement to print out whether the portfolios total savings is enough for an emergency fund

-- Part 2 Retirement Planning
1. Then will set all variables for the alpaca.get_barset for SPY and AGG then run and print it 
2. Then will configuring a Monte Carlo simulation to forecast 30 years cumulative returns and print portfolio data 
3. Then run the Monte Carlo simulation 
4. Then plotting Monte Carlo simulation in line plot and save as new variable and also saving image to directory 
5. Then will make a distribution plot with Monte Carlo Simulation will save as new variable and also saving image to directory
6. Retirement analysis, will summarize cumulative returns 
7. Calculate the range of possible outcomes with the upper and lower 95% with out initial investment, print range 
8. Repeat step 7 for a 50% increase in initial investment, print range 

-- Part 3 Optional Challenge - Early Retirement 
1. Repeat part two will just change Monte Carlo Simulation for 5 year analysis and 10 year analysis 
2. Then will also manipulate weights of the portfolio and change initial investments


All Requirements are met as seen in the requirements below:

Requirements

Personal Finance Planner  (35 points)

To receive all points, your code must:

Collect crypto prices using the requests Library. (10 points)
Collect investments data using Alpaca: SPY (stocks) and AGG (bonds). (10 points)
Perform a savings health analysis. (15 points)


Retirement Planning (35 points)

To receive all points, your code must:

Complete a Monte Carlo Simulation with 500 runs. (15 points)
Plot the Monte Carlo simulation results. (5 points)
Plot the probability distribution and confidence intervals. (5 points)
Complete the retirement analysis. (10 points)


Optional Bonus (10 points)

To receive all bonus points, your code must:

Optional: Adjust the portfolio to reflect an early retirement and rerun the analysis to show either a higher stock than bond ratio, or to have a higher initial investment. (10 points)


Coding Conventions and Formatting (10 points)

To receive all points, your code must:

Place imports at the beginning of the file, just after any module comments and docstrings and before module globals and constants. (3 points)
Name functions and variables with lowercase characters and with words separated by underscores. (2 points)
Follow Don't Repeat Yourself (DRY) principles by creating maintainable and reusable code. (3 points)
Use concise logic and creative engineering where possible. (2 points)


Deployment and Submission (10 points)

To receive all points, you must:

Submit a link to a GitHub repository that’s cloned to your local machine and contains your files. (5 points)
Include appropriate commit messages in your files. (5 points)


Code Comments (10 points)

To receive all points, your code must:

Be well commented with concise, relevant notes that other developers can understand. (10 points)

