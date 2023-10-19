# Olympic-Games-Analysis
The completed dashboard includes visualizations and filters that provide viewers a simple way to browse the summer games through time. Some options include using the year as a filter for time, utilizing the nation code to concentrate on a single nation, or examining a competitor or a particular sport across time.

The Main goal is to visualize data that will help readers understand how countries have performed historically in the summer Olympic Games.
The primary objective is still to provide historical performance data for many nations, with the option to select the country you represent.

Data Model

![bidatamo](https://github.com/ChristianMmcly/Olympic-Games-Analysis/assets/117743442/416e9e1e-f121-4e32-90f2-f5f7c1b73627)

Calculation
Using DAX (Data Analysis Expressions), the Power BI reports were built with the calculations listed below. The reuse of measurements (measure branching) was emphasized in order to reduce the amount of coding:
Number of Competitors:
# of Competitors = DISTINCTCOUNT( ‘Olympic Data'[ID] )
# of Medals = COUNTROWS( ‘Olympic Data’ )
# Of Medals (Registered) = CALCULATE( [# of Medals], FILTER( ‘Olympic Data’, ‘Olympic Data'[Medal] = “Bronze” || ‘Olympic Data’ [Medal] = “Gold” || ‘Olympic Data'[Medal] = “Silver” ))

Olympic Games Analysis Dashboard
The completed dashboard has filters and visual that make it simple for end users to search through past summer games based on year, nation, competitor name, and sport category. These will enable users to gain a thorough knowledge of how various nations have performed at the Summer Olympic Games over time.
Users can now apply filters to learn more about their competitors' and their nation's performance.

![bidash](https://github.com/ChristianMmcly/Olympic-Games-Analysis/assets/117743442/4b893ba9-f5ce-40aa-845e-2262c69b7b39)
