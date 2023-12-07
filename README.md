# Home_sales

# DataFrame Creation
  In the beginning of my code I used sparkcontext to be able to read my CSV file and then I created it into a starting dataframe to house all the data. I then used a createOrReplace function so I have a temporary veiw of the DataFrame.

# Results Search
  To find the average price for a four bedroom house sold for each year, I used the sql function within my spark variable and find the date with the price from my temporary dataframe and output the average price of all the 4 bedroom houses grouped together and sorted by date. I then did around the same thing for finding the average price of a house that was built with 3 bedrooms and 3 bathrooms.  My specific wording for my sql function was to find the date built and round all the housing prices together from my dataframe where where bedrooms and bathrooms equaled 3 and then had it group and order by date built.  The next search I did was on the average price of a home with 3 beadrooms and bathrom but also had two floors.  my sql function was relativley the same as the first search but I added an AND search to find all the houses with 2 floors and had at least 2,000 square feet of space.  My last search was jsut looking for the average price of the home on anything over $350,000 and i printed the time that it took for the query to run.

# Caching and Closing 
At the end of my notebook I cached the data to parquet it and then had it read that way so it woudl be formatted better.  After I had a better view I uncached the table to make sure that the cache was no longer running at the end notebook.
