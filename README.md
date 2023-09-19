# data-collection-challenge

"You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.
As you work on this Challenge, remember that you’re strengthening the same core skills that you’ve been developing until now: collecting data, organizing and storing data, analyzing data, and then visually communicating your insights."

The following questions were investigated using the scraped data:

• How many months exist on Mars?
  > 12, or 24, depending on calendar system used and reference material

• How many Martian (and not Earth) days worth of data exist in the scraped dataset?
  > 1867 sols

• What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question: 
  > The third Earth month of the dataset routinely was coldest and 8th month was the hottest.
  > Darian calendar showed month 22 (Tula) as the coldest and 8 (Meena) as the hottest.

  Bar charts of the data sorted and unsorted in notebook.

• Which months have the lowest and the highest atmospheric pressure on Mars?
  > The sixth Earth month of the dataset routinely had the lowest atmospheric pressure while the ninth month had the highest.
  > Darian calendar showed month 3 (Dhanus) as the lowest pressure and 10 (Mesha) as the highest.

  Bar charts of the data sorted and unsorted in notebook.
  
• About how many terrestrial (Earth) days exist in a Martian year? 
  > A Martian year is the amount of time it takes for Mars to orbit the sun, of course, and the number of sols in a Martian year are going to differ from an Earth day.  The cyclical nature of this orbit will show up in the data if temperature is plotted against a continuous timeline.  The same trend occurs with Earth and behaves in the form of regional seasons - cold winters, warm summers, etc.  Plotting solar longitude against time as well, a very stark sawtooth pattern arises in a regularly repeating pattern.  Given the nature of the solar longitude and the relatively short distance the Curiosity rover was built to ravel, this corroborates the data, showing a period on a similar order to the temperature.
  > Terrestrial days are provided by the dataset as well as the local temperature recorded by Curiosity.  Seasonality can indeed be observed in the data.  Conveniently it appears that the start of a Martian year coincided with the Earth year 2013, the next temperature peak can be observed approximately 80% of the way into the year 2014.
Earth years are 365 days, thus an elapsed time of 365 + 0.8*365 yields an estimated 657 sols per Martian year.  

  > The generous Nasa Aerospace engineer Thomas Gangale corroborates this finding in detail, showing a more accurate count at 668.5921 sols.  Pretty close.

Sources used for assistance:
https://ops-alaska.com/time/gangale_mst/darian.htm#:~:text=Since%20the%20Darian%20calendar%20year,Earth%20or%20Mars)%3F%22
https://stackoverflow.com/questions/32888124/pandas-out-of-bounds-nanosecond-timestamp-after-offset-rollforward-plus-adding-a
