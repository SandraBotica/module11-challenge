# module11-challenge

Part 1 Questions

        In the <part_1_mars_news.ipynb>, You will find the code used to scrape the Mars News website.
        I have stored the title and preview text in a python dictionary and stored the pythoin dictionaries into a python list.
        This scraped data has also been saved to <mars_news_json.json>.

Part 2 Questions

        In the <part_2_mars_weather.ipynb>, You will find the code used to scrape and analyse the Mars Weather Data.

How many months are there on Mars?
        12

        In this scraped dataset the first row is ["sol"]= 10 and ["month"]= 6
        then @ ["sol"]= 668, the first sol for ["month"]= 6 appears again
        then @ ["sol"]= 1337, the first sol for ["month"]= 6 appears again
        with the last row of data @ ["sol"]= 1977 the last sol for ["month"]= 5
        Making me deduce that the dataset has 3 years of data, with one year being the 12 martian months of sol days.

How many Martian days' worth of data are there?
        1867

        The first row is ["sol"]= 10 and the last row is ["sol"]= 1977
        This makes me think that there are 1977-10 = 1967 sol days in the dataset.
        When you look at the first 9 rows  the sol days increment from 10,11,12,13,14,15,16,17 and the next row is 21.
        This indicates that sol day 18,19,20 do not have data recorded for that sol day on Mars.

        Considering there is 1867 rows of data and 1967 sol days in the dataset.
        One may deduce that 1967 sol days - 1867 rows, that there is 100 sol days of data missing in this dataset.

What is the average low temperature by month?
        
        Plot the average temperature by month
        I have saved the plot in the <Images> folder file title is <AveragePressureMonth.png>

        Identify the coldest and hottest months in Curiosity's location

        Coldest Month 3 -83.31
        Hottest Month 8 -68.38

Average pressure by Martian month.

        Plot the average pressure by month
        I have saved the plot in the <Images> folder file title is <AveragePressureMonth.png>

        Which months have the lowest and the highest atmospheric pressure on Mars? 
        The month with the lowest average atmospheric pressure on Mars was Month 6, recording an average of 745.05 (atm)
        The month with the highest average atmospheric pressure on Mars was Month 9, recording an average of 913.31 (atm)

How many terrestrial (earth) days are there in a Martian year?

        ~625 terrestrial (earth) days in a Martian year based on the plot of min-temp.
        or
        ~664 terrestrial (earth) days in a Martian year.
        This is based on scrolling through sol and month columns in data, explained below

        Looking at the plot above I find the first highest point on the graph (highest min temperature) and check what day it might be on the x_axis, ~day 125, then find the next highest point on the graph (highest min temperature) and check what day it might be on the x_axis, ~day 750.

        Based on this I deduce that there are ~ 625 terrestrial (earth) days in a Martian year.

        The other thing to consider is this:
                Having scrolled through the 'sol' column data
                The first row = sol 10 month 6
                then at sol 668 month 6 (the next 1st sol day of month 6)
                then at sol 1337 month 6 (the next 1st sol day of month 6)
                then at sol 1977 month 5 (could be more sol day for 5th month after last row)
                So
                668-10 sol days = 658 sol days in a year
                1337-668 sol days = 669 sol days in a year
                Average of these 2 values is 663.5
                

Export the DataFrame to a CSV file.

        I have saved the scraped data in the images folder file title is <data.csv>

Enjoy marking this assignment.
Thank you.
Sandra