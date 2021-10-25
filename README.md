# challenge_5
## Project Overview

This Python notebook has two parts. Part 1 consists of financail planning for emergencies and Part 2 is a planner for retirement.

---

## Technologies

The application is in python and is uing the following libraries:

* [os](https://github.com/python/cpython/blob/main/Lib/os.py) - For pulling in the key.

* [pandas](https://pandas-profiling.github.io/pandas-profiling/docs/master/index.html) - For data analysis.

* [load_dotenv](https://github.com/motdotla/dotenv) - to load in an env file.

* [%matplotlib](https://github.com/ipython/matplotlib-inline) - For output of plotting commands.

* [requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) - Pull rquests for data to be pulled in the notebook.

* [json](https://github.com/bradjasper/ImportJSON) - To read json files as python.

* [tradeapi](https://github.com/alpacahq/alpaca-trade-api-python) - For pulling in the keys and version.

* [MCSimulation]-Simulation provided by the teacher. Will be attached to Github.


The operating system used in creating the application is Windows 10 64 bit. The application that used to code in notebook is Jupyter and then tested in Gitbash and Terminal. 

The application is depend on excel file 'top.env' for API keys and URLs

The output files were:

```python
load_dotenv("top.env")
```

```python
btc_url = "https://api.alternative.me/v2/ticker/Bitcoin/?convert=USD"
eth_url = "https://api.alternative.me/v2/ticker/Ethereum/?convert=USD"
```
```python
alpaca = tradeapi.REST(
    alpaca_api_key,
    alpaca_secret_key,
    api_version="v2")
```
---

## Installation Guide

1. Open Gitbach or terminal and go ito the folder where you want to place the files.
2. Click on the blue "code" button which will allow you to clone.![<Code button in Github>]()
3. Then click on SSH or HTTPS as a clone method depending on if you have the SSH key setup. You will copy the link. You will then type "git clone" in Gitback or Terminal. Then paste the ssh or https information and press enter.
4. Next type "git pull" command in Temrianl or GitBash to pull the repository from the remote Github repository to a local directory on your computer.
5. You have access to the application. Also there will be all the python files that the application is depended on. 

---

## Usage

Below is a list of steps/analysis seen in the notebook:
    1.Part 1
        1. Evaluate the Cryptocurrency Wallet by Using the Requests Library
            1.Create a variable named monthly_income, and set its value to 12000
            2. Use the Requests library to get the current price (in US dollars) of Bitcoin (BTC) and Ethereum (ETH) by using the API endpoints that the starter code supplied
            3.Navigate the JSON response object to access the current price of each coin, and store each in a variable.
            4.Calculate the value, in US dollars, of the current amount of each cryptocurrency and of the entire cryptocurrency wallet.
        2. Evaluate the Stock and Bond Holdings by Using the Alpaca SDK
            1.In the Starter_Code folder, create an environment file (.env) to store the values of your Alpaca API key and Alpaca secret key.
            2.Set the variables for the Alpaca API and secret keys. Using the Alpaca SDK, create the Alpaca tradeapi.REST object. In this object, include the parameters for the Alpaca API key, the secret key, and the version number.
            3.Set the following parameters for the Alpaca API.
            4.Get the current closing prices for SPY and AGG by using the Alpaca get_barset function. Format the response as a Pandas DataFrame by including the df property at the end of the get_barset function.
            5.Navigating the Alpaca response DataFrame, select the SPY and AGG closing prices, and store them as variables.
            6.Calculate the value, in US dollars, of the current amount of shares in each of the stock and bond portions of the portfolio, and print the results.
        3.Evaluate the Emergency Fund
            1.Create a Python list named savings_data that has two elements. The first element contains the total value of the cryptocurrency wallet. The second element contains the total value of the stock and bond portions of the portfolio.
            2.Use the savings_data list to create a Pandas DataFrame named savings_df, and then display this DataFrame. The function to create the DataFrame should take the following three parameters.
            3.Use the savings_df DataFrame to plot a pie chart that visualizes the composition of the member’s portfolio. The y-axis of the pie chart uses amount. Be sure to add a title.
            4.Using Python, determine if the current portfolio has enough to create an emergency fund as part of the member’s financial plan. Ideally, an emergency fund should equal to three times the member’s monthly income.
    2. Part 2
        1.Make an API call via the Alpaca SDK to get 3 years of historical closing prices for a traditional 60/40 portfolio split: 60% stocks (SPY) and 40% bonds (AGG).
        2.Run a Monte Carlo simulation of 500 samples and 30 years for the 60/40 portfolio, and then plot the results.The following image shows the overlay line plot resulting from a simulation with these characteristics. However, because a random number generator is used to run each live Monte Carlo simulation.
        3.Plot the probability distribution of the Monte Carlo simulation. Plot the probability distribution of the Monte Carlo simulation. The following image shows the histogram plot resulting from a simulation with these characteristics. However, because a random number generator is used to run each live Monte Carlo simulation.
        4.Generate the summary statistics for the Monte Carlo simulation.
---

## Contributors

This application was provided by the instrutor of Columbia University and addtional code was added by Khatija Azeem to complete the project.

---

## License

For this application, I used Github to uplaod the file into a repository. Since this is a public file, there will be no restriction on usage of this code. 