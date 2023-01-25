# TMDB Movie Franchises
An analysis of movie franchises using TMDB's API


## Summary
This project sought to explore the landscape of the franchise film market. Using data pulled from the popular site, The Movie Database, I analyzed a variety of attributes of films and their respective franchises. I looked at the relationships between factors such as budget, revenue, genre, and user engagement. I arrived at a “success equation” that defines the ultimate revenue-generating franchise. Future exploration will include a predictive model and digging deeper into audience demographics.

### Tools Used
Python (and Pandas), Microsoft Excel, Tableau

### Skills Employed
API calls, vlookup, pivot tables, analysis, visualization, correlation matrix, data cleaning, data transformation

### Resources
[Project Page](http://teriandony.com/projects/movie-franchises/)

[Tableau Visualizations - Main Analysis](https://public.tableau.com/views/TMDBMovieFranchisesAnalysis/Story1?:language=en-US&:display_count=n&:origin=viz_share_link)

[Tableau Visualizations - Genre Dashboard](https://public.tableau.com/views/TheMovieDatabaseGenrePerformanceAnalysis/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)

[TMDB API Documentation](https://developers.themoviedb.org/3/getting-started)

[Google Slides Presentation](https://docs.google.com/presentation/d/176ti1AUvek9AeFiJ7ABlCiyP5QxIJyusoyLYDwmUECQ/edit?usp=sharing)

### A note on the CSV files
I've provided two CSV datasets. "tmdb_data_final" is best used for genre analysis. "tmdb_data_unique" should be used for all other analyses.
This is because each movie can list more than one genre (eg, Star Wars is "action", "adventure" and "sci-fi"). I exploded the dataframe in Python so that each genre was its own row. Meaning, Star Wars had three rows and the only unique field between them was genre. This wouldn't give accurate information for fields like revenue and budget (which would sum all three rows together). So, I created the unique dataset for all other analyses other than genre. This dropped duplicate rows and kept only one row per movie.
