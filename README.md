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
      * Project_1_Data_Cleaning
      * Project_1_Exploratory_Plots
      * Project_1_VADER
  * DATA
      * jo.csv - original data for Jonathan Owens
      * sb.csv - original data for Simone Biles
      * clean_jo - clean data for Jonathan Owens
      * clean_sb - clean data for Simone Biles
      * Data Appendix
  * OUTPUT
      * Comment_Length_Scatter
      * Jonathan_Owens_Comment_Dates
      * Jonathan_Owens_Sentiment_Analysis
      * Jonathan_Owens_Word_Cloud
      * Simone_Biles_Comment_Dates
      * Simone_Biles_Sentiment_Analysis
      * Simone_Biles_Word_Cloud
  * REFERENCES
      * [1] E. Giambalvo, “Simone Biles dazzles with difficulty, but execution makes her unstoppable,” Washington Post, Oct. 05, 2023. Available: https://www.washingtonpost.com/sports/olympics/2023/10/05/simone-biles-gymnastics-scores-execution/. [Accessed: Jan. 30, 2024]

      * [2] “USA Gymnastics | Skills Named for U.S. Gymnasts.” Available: https://members.usagym.org/pages/gymnastics101/skillsNamed.html. [Accessed: Jan. 30, 2024]

      * [3] “Jonathan Owens Stats, News and Video - DB,” NFL.com. Available: https://www.nfl.com/players/jonathan-owens/. [Accessed: Jan. 30, 2024]

      * [4] “New Packers safety Jonathan Owens playing with ‘chip on my shoulder’ after starting career undrafted,” NFL.com. Available: https://www.nfl.com/news/new-packers-safety-jonathan-owens-playing-with-chip-on-my-shoulder-after-startin. [Accessed: Jan. 30, 2024]

      * [5] “Simone Biles reacts to backlash over husband Jonathan Owens saying he didn’t know her before they dated,” TODAY.com, Dec. 24, 2023. Available: https://www.today.com/popculture/jonathan-owens-simone-biles-how-they-met-rcna130830. [Accessed: Jan. 30, 2024]

      * [6] “Features and Updates — VaderSentiment 3.3.1 documentation.” Available: https://vadersentiment.readthedocs.io/en/latest/pages/features_and_updates.html. [Accessed: Jan. 30, 2024]

      * [7]
“Instagram Comment Scraper.” Available: https://chromewebstore.google.com/detail/instagram-comment-scraper/ldhjpljmgnggmkpcgaicmocfoefbcojl?hl=en-GB&pli=1. [Accessed: Feb. 08, 2024]
      * [8]
“Welcome to VaderSentiment’s documentation! — VaderSentiment 3.3.1 documentation.” Available: https://vadersentiment.readthedocs.io/en/latest/. [Accessed: Feb. 08, 2024]

 
## Section 3: Instructions for reproducibility
1. Preprocessing
In order to collect sentiment data from Instagram posts after Jonathan Owens’ interview on The Pivot, the profiles of Simone Biles and Jonathan Owens need to be accessed. This involves searching their profiles on Instagram and choosing an equal number of posts dated December 19, 2023 and after from each profile, as well as their "pinned" posts. Posts where the user limited comments can be excluded. After the data has been identified, it can be downloaded for further analysis. For the sake of our analysis, we scraped comments from the three posts made by each individual made immediately following December 19, 2023 and each of their three pinned posts. In total, the comments were scrapped from 6 posts each. 
2. Scraping Data from Instagram
Comments on each Instagram post will be scraped using the chrome extension “Instagram Comment Scraper.” This allows 100 comments per post to be downloaded as a CSV. For each individual, six posts need to be scraped meaning there will be a total of 600 comments scraped. When downloading, name the files sb1.csv, sb2.csv, etc. for the Simone Biles exports and jo1.csv, jo2.csv, etc. for the Jonathan Owens exports. 
4. Cleaning Data
Observe data for each individual. The intial data cleaning that needs to take place is combining all of the scrapped instagram comments into a single data set for each individual. To do so, place each of the 12 downloaded csv files into the scripts folder and run the **Project _1_Data_Cleaning.ipynb** file in the **SCRIPTS**. The usable data sets will be output to the **DATA** folder. Cleaning data includes changing "Publish Date" to only include the date rather than the date AND time of each comment. The next step would be to drop rows with missing values. All of this cleaning will happen in the **Project_1_VADER.ipynb** file. 
4. Sentiment Analysis
The Vader sentiment analysis package on python will be used to analyze all of the Instagram comments. Positive, negative, and neutral sentiment scores will then be created and appended to the original dataset. To run the analysis run all cells of the **Project_1_VADDER.ipynb** file in the **SCRIPTS**. 
