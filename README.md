# module11-challenge

Part 2 Questions
1. How many months are there on Mars? 
        
        12

        In this scraped dataset the first row is ["sol"]= 10 and ["month"]= 6
        then @ ["sol"]= 668, the first sol for ["month"]= 6 appears again
        then @ ["sol"]= 1337, the first sol for ["month"]= 6 appears again
        with the last row of data @ ["sol"]= 1977 the last sol for ["month"]= 5
        Making me deduce that the dataset has 3 years of data, with one year being the 12 martian months of sol days.

2. How many Martian days' worth of data are there?

        1867

        The first row is ["sol"]= 10 and the last row is ["sol"]= 1977
        This makes me think that there are 1977-10 = 1967 sol days in the dataset.
        When you look at the first 9 rows  the sol days increment from 10,11,12,13,14,15,16,17 and the next row is 21.
        This indicates that sol day 18,19,20 do not have data recorded for that sol day on Mars.

        Considering there is 1867 rows of data and 1967 sol days in the dataset.
        One may deduce that 1967 sol days - 1867 rows, that there is 100 sol days of data missing in this dataset.

3. What is the average low temperature by month?
        
        Plot the average temperature by month
        I have saved the plot in the images folder file title is AveragePressureMonth.png


        Identify the coldest and hottest months in Curiosity's location

        Coldest Month 3 -83.31
        Hottest Month 8 -68.38

4. Average pressure by Martian month.

        Plot the average pressure by month
        I have saved the plot in the images folder file title is AverageTemperatureMonth.png

        Which months have the lowest and the highest atmospheric pressure on Mars? 
        The month with the lowest average atmospheric pressure on Mars was Month 6, recording an average of 745.05 (atm)
        The month with the highest average atmospheric pressure on Mars was Month 9, recording an average of 913.31 (atm)

5. How many terrestrial (earth) days are there in a Martian year?

        ~600 terrestrial (earth) days in a Martian year

        Looking at the plot above I find the first highest point on the graph (highest min temperature) and check what day it might be on the x_axis, ~day 125, then find the next highest point on the graph (highest min temperature) and check what day it might be on the x_axis, ~day 750.

        Based on this I deduce that there are ~ 600 terrestrial (earth) days in a Martian year.

6. Export the DataFrame to a CSV file.

        I have saved the scraped data in the images folder file title is data.csv