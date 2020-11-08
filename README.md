# Building a fanbase

In this first project, I'm going to analyze the film industry using datasets from IMDb.com. The goal is to explore the data and help Microsoft's Team to understand the market and elaborate a strategy to enter this industry.

**Why looking only at IMDb data?**

From all provided datasets, IMDB.com was the only source that had several files and a lot of information from different levels. I could try to merge all different sources but since they don't share the same `title_id` it would be difficult to merge using `movie_title`. So for simplicity, I'm limiting my analysis to one source.

_Caveat about IMDb's datasets: It seems like the files were extracted in 2019 based on the No. of Movies over time. Therefore, more work could be done on getting updated data._

## Navigation

You can find the following files/folders in my repository:

### `Film Industry Analysis.ipynb`

- **Content:** Main Jupyter Notebook with the whole analysis.

- **What I'm doing:**
  1. Unzipping files and exporting them to a different folder.
  2. Exploring the available datasets, understanding what's available, and the structure/granularity/pitfalls of each dataset.
  3. Asking questions that will help Microsoft's team understand the industry, then answering them using datasets and developing recommendations based on my findings.
  4. Presenting results/conclusions through visualizations.

### `zippedData/unzippedData` folders

- **Content:**
  - Zipped/unzipped files from the following sources:
    - [Box Office Mojo](https://www.boxofficemojo.com/)
    - [IMDB](https://www.imdb.com/)
    - [Rotten Tomatoes](https://www.rottentomatoes.com/)
    - [TheMovieDB.org](https://www.themoviedb.org/)
  - **Context:** Those are well-known movie websites with a lot of information related to movies, tv-shows, video games, and streaming content - including cast, ratings, movie length, titles in different places, budget, trivia, goofs, rankings, personal biographies, plot summaries, and fan and critical reviews.

## Analysis Approach

The datasets provide a lot of useful information. However, to develop a strategy to enter the film industry, I'd like to find trends in successful movies, which means that first I need to define success.

### Definition of success and how to measure it

Success can be defined in many ways, but I suppose that Microsoft would like to have popular movies with high views, ratings, and maybe profits. It's hard to expect that their first venture will be popular, let alone profitable.

Consequently, I will measure success based on the **Number of Votes** and **Ratings**. Unfortunately, I'm limited to what's available, and the number of votes might not be an ideal proxy for views, but it's the closest I can get.

From my perspective, **Number of Votes** can be even more valuable because differently from a view where it's just one person watching a movie, a vote means that someone went to IMDb's website, created a profile/logged in, searched for the film and voted. Since we have all these steps to complete to vote, I'd say that votes are more meaningful.

## Questions

Below you can find the questions I raised during the project. I'll also add an explanation for why I think those are valid and important.

**1. Is the number of new movies growing over time?**

>**Reason:** We must understand whether this is a market that is producing more and more content over time.
>
> If Microsoft is thinking about entering the Film Industry, this question will give a good understanding of **whether it's a growing industry** and if there's **a lot of competition**. It's expected that if the **supply of movies is increasing**, the **demand is going in the same direction**, so it's probably a good market to enter.

**2. Which `genres` have the most movies?**

>**Reason:** By answering this question, I can understand a bit more about the demand. I believe that producers would not create movies of `genres` that are not popular.
>
>Having this information helps Microsoft to understand the market and start thinking about which strategy to apply (compete with the popular genres or focus on others/not so saturated genres).

**3. Which `genres` have consistently had the most No. of movies over time?**

>**Reason:** With this question, I can find trends of `genres` that are becoming more popular over time and maybe suggest Microsoft follow the same trends.

**4. What are the best/most rated `genres`?**

>**Reason:** So far, I have done most of my analysis using No. of Movies. This time, I'm going to use No. of Votes.
>
>I think that Ratings/Number of Votes can be more meaningful because **the act of voting requires someone to go to IMDB.com, search for the movie, and vote.** Therefore, I'd say that it gives us a **good understanding of the market from the consumers' standpoint**. Also, **if someone voted, it's because they watched the film, so the number carries more meaning.**
>
>Therefore, by asking this question, we get a different perspective on `genres` and a **good idea of which one would have a higher chance of success.**

**5. Which roles are the most important in a movie?**

>**Reason:** The idea of this question is to **understand which roles require more attention** or are more likely to **bring more views/votes to movies**. Maybe there are some similarities among successful films.
>
>By knowing which roles bring more votes, **Microsoft can plan their budget accordingly or dedicate more time to find the best on important roles.**

**6. What's the impact in terms of the popularity of having a movie playing internationally?**

>**Reason:** This question aims to understand whether Microsoft should also focus on making the movie **famous internationally** or if most of the popular films didn't necessarily were played in different countries.
>
>By launching a film in different countries, there's much preparation and other things to consider (Marketing Material, Subtitles, Local Titles, etc.). So knowing this ahead of time is helpful.

## Conclusions

**1. The Film Industry is a competitive and growing market:** The supply of new movies is increasing over the years. The reason for that can be the following:

- Movies have become cheaper to make over time as technology became more accessible to anybody.
- The market and customer base grew. So the demand for more content is growing.
- People have access to the internet + Consumers are moving from Cable TV to On-Demand subscriptions.

Those are all positive reasons for Microsoft to enter the Film Industry. The only problem is that competition has grown a lot, and Microsoft will compete with Apple, Netflix, Disney, Amazon, and YouTube. Moreover, there's a lot of discussions on the subscription market's saturation, so their pricing will have to be competitive.

**2. Documentary, Drama, and Comedy are the most popular genres in No. of Movies:** After analyzing movies in IMDb's database, it's possible to see significant numbers of `Documentaries`, `Drama` and `Comedy` movies. When looking at different combinations of genres, `Comedy + Drama` and `Comedy + Drama + Romance` have had the most No. of Movies over the last ten years. For Microsoft, these might be too saturated genres to enter but show a picture of the industry.

**3. Building a Fanbase:** During the analysis of the Most Voted/Best Rated movies, `Action, Adventure, Sci-Fi`, `Adventure, Animation, Comedy` and `Action, Adventure, Fantasy` showed up a lot over the last ten years. Those were the `genres` with the most No. of Movies in the Top 1% of movies in terms of number of votes. <br>I think the reason is that most of these movies are **superhero movies (Captain America, Iron Man 2, Thor, and Wonder Woman)**, part of a **movie series (Avengers, Star Wars, Pirates of the Caribbean, Toy Story, Despicable Me)** or **Pixar Movies**. <br> **They attract a lot of fans over time. So once you have that fanbase, it becomes easier to create movies with a lot of views, votes and become popular.** <br>
Therefore, a good strategy for Microsoft might be to enter this world and try to **partner with another company** like DC/Marvel and create an exclusive superhero series. The good thing about a partnership is that they wouldn't have to develop a new story since they would use an existing character. <br>Also, another option would be to develop a new `Adventure, Animation, Comedy` story with **unique characters like Minions on Despicable Me.** This one is a bit harder to execute, though.

**4. Hire the best on roles that matter the most:** After analyzing **which roles were the most frequent in high voted movies**. The recommendation is to **focus on getting the best actors, then writers, producers, actresses, and directors**. _Note: Unfortunately, this analysis is biased towards men since actors have higher importance relative to actresses. And the reason is that there are more actors in high voted movies. I'd probably group both as the same to avoid adding this type of bias._

**5. Have an international footprint:** The **Average No. of Votes increases as the No. of Regions in which the movie is played increases**. Therefore, my recommendation for Microsoft would be to prepare to **launch the film internationally**.

## Final Thoughts

More could be done to gather more insights. For example, I'd like to see the number of Tickets Sold, viewers + demographics, and more information on which Platform/Studio created the movie. Moreover, understanding Microsoft's goals would also guide my analysis to relevant conclusions for them. For example, I don't know if they're trying to be profitable in this endeavor or if the goal is to enter this industry and then worry about profitability.
