# Project1-DS-4002
Welcome to our Project 1 info!

## Contents of our repository:
> Section 1: Software and platforms

> Section 2: Map of documentation

> Section 3: Instructions for reproducibility

## Section 1: Software and platforms
* Software
  * Visual Studio Code
  * Google Colab
  * Instagram
  * Instagram Comment Scraper (Google Chrome Extension)
* Packages needing installation
  * pandas
  * numpy
  * matplotlib.pyplot
  * vaderSentiment, SentimentIntensityAnalyzer
* Platforms
  * Windows
  * Mac
 
## Section 2: Map of documentation
* Project1-DS-4002
  * README.md
      * Orientation of repository
  * LICENSE.md
      * Terms and conditions
  * SCRIPTS
      * LIST ALL NAMES OF FILES
      * Project_1_Master_Script
  * DATA
      * jo.csv - original data for Jonathan Owens
      * sb.csv - original data for Simone Biles
      * clean_jo - clean data for Jonathan Owens
      * clean_sb - clean data for Simone Biles
      * Data Appendix
  * OUTPUT
      * Figures
      * Tables
      * Word Clouds
  * REFERENCES
 
## Section 3: Instructions for reproducibility
1. Preprocessing
> In order to collect sentiment data from Instagram posts after Jonathan Owens’ interview on The Pivot, the profiles of Simone Biles and Jonathan Owens need to be accessed. This involves searching their profiles on Instagram and choosing an equal number of posts dated December 19, 2023 and after from each profile, as well as their "pinned" posts. Posts where the user limited comments can be excluded. After the data has been identified, it can be downloaded for further analysis. For the sake of our analysis, we scaped comments from the three posts made by each individual made immediately following December 19, 2023 and each of their three pinned posts. In total, the comments were scrapped from 6 posts each. 
2. Scraping Data from Instagram
> Comments on each Instagram post will be scraped using the chrome extension “Instagram Comment Scraper.” This allows 100 comments per post to be downloaded as a CSV. For each individual, six posts need to be scraped meaning there will be a total of 600 comments scraped. 
3. Cleaning Data
> Observe data for each individual. Cleaning data includes changing "Publish Date" to only include the date rather than the date AND time of each comment. The next step would be to drop rows with missing values.
4. Sentiment Analysis
> The Vader sentiment analysis package on python will be used to analyze all of the Instagram comments. Positive, negative, and neutral sentiment scores will then be created and appended to the original dataset.
