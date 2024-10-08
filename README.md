# Best Picture winners are rarely a box office hit

## Description of what I aimed to accomplish: <br>
I wanted to investigate how much Best Picture winners make at the box office compared to the top-grossing movies. 

## Description of findings: <br>
- I assumed that streaming services would make the revenue of the top-grossing movies go down but they have actually increased over the last few decades. Even after a dramatic drop in 2020 (because of the COVID-19 pandemic), the industry still managed to pick itself back up with 'Spiderman: No Way Home' becoming the second-highest grossing film ever. <br>
- From 1995, 'Titanic' and 'Forrest Gump' were the only Best Picture winners that have were also the most-grossed film of that year.<br>
- 'Oppenheimer' is the first Best Picture winner in ten years to gross over $100 million USD (the last film that did that was 'Argo').<br>
- On average, top-grossing movies grossed 13 times more revenue than Best Picture winners at the Oscars (from 2014 - 2023).<br>

## Data collection and analysis process: <br>
The data collection process was arduous. Initially, I scraped Billboard's website of the Top-Grossing Films for Each Year (https://www.billboard.com/lists/top-grossing-films-each-year/) but then realised the page was out of date so did not use that data. I used box office mojo data instead, which is where Billboard got their old data from in the first place. I manually searched every Oscar Winner up to Rocky in 1977 and put the data into a list of dictionaries. <br>

Once I did that I moved onto scraping this website for the domestic gross of the top-grossing movies: https://www.boxofficemojo.com/year/. It took me a while to realise that the Total Gross listed in the table is the Total Gross of ALL the movies that came out that year, not just the top-grossing movie of that year. I realised that was the case when I plotted my data onto Flourish and realised the numbers for Titanic were vastly different when they should have been the same considering it was top-grossing movie that year AND the Oscar winner. Since the format of the website looked identical for each movie's page, I used a for loop and scraping to go through each link and find the domestic gross for each movie listed in that table. All the data was accurate except for Forrest Gump, for some reason it was not listed in the table with top grossing movies despite having a higher domestic gross but I spotted that error quite quickly because I knew there shouldn't be any gold coin bars higher than silver coin bars. 

Once I scraped and cleaned the data I merged it all into one dataframe. I analysed the data using pandas and plotted the results in Flourish.

## Data Visualisation: <br>
I downloaded some free vectors (Coins and Oscars) and edited them to make some high quality visuals for the title slide as well as matching charts. 

## Where you grew the most during the project: <br>
I got more comfortable with scraping and data cleaning techniques (.replace, .strip, and a bit of regex). I also got a lot more comfortable with illustrator to make the visualisation look appealing.

## Things I tried to do or wanted to do but did not have the skills/time: <br>
I tried to do ai2html scrollytelling again but could not get it to work so I resorted to doing it with images instead. I also would've loved to make parts of the visuals animated but I had no idea where to start and didn't have time to teach myself that.
