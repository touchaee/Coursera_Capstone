# Where to open a new Thai restaurant in New York?

Table of Contents
[1. Introduction: Business Problem](#Introduction: Business Problem)
2. Data
3. Methodology
4. Analysis
5. Results and Discussion
6. Conclusion

## Introduction: Business Problem

Over the last 20 years, Thai restaurants have been one of the fastest-growing dining categories in New York City. Ever since the advent of places specializing in regional cuisines, often presenting recipes not seen here before, the Thai dining scene has been more exciting than ever before. So that now I have the fiery food of Isan in the northeast, the mellower food of Chiang Mai near the Burmese border, oodles of noodles from Sukhothai, the curries of central and southern Thailand, the urban cuisine of Bangkok, and the Malaysian-leaning food of the peninsula. Our newest arrival is the food of the capital's Chinatown.

But the pandemic has been tough on Thai restaurants, a one-third have closed, mostly as a result of the pandemic. The good news is that new places have arisen to replace them; in fact, Thai has been most prominent in the category of new restaurants, as will be shown in what follows, along with lots of highly recommended old favorites.

This project aims to find a location for the opening of a Thai restaurant in NY, Specifically, this report will be targeted to stakeholders interested in opening a Thai restaurant in New York City.

The first task would be to find the areas lack Thai Restaurants by analyzing restaurant data from FourSquare API and shortlisting an area, where Thai restaurant is not amongst the most common venues.

I will make use of our data science tools to analyze data and focus on the areas and explore its areas and the 10 most common venues in each area so that the best areas where Thai restaurant is not amongst the most common venue can be selected.

## Data
Based on the definition of our problem, the factors that will influence our decision are:
- finding the areas lack Thai Restaurants
- finding the most common venues
- Choosing the right neighborhood within the borough

I will be using the geographical coordinates of NY to plot restaurant in a neighborhood that is lack of Thai Restaurant and in the city's vicinity, and finally, cluster our neighborhoods and present our findings.

Following data sources will be needed to extract/generate the required information:

- **Part 1: Using an IBM dataset containing the New York Borough, Neighborhood and geometry coordinates**: A dataset consisting of Borough, Neighborhood, Latitude, and Longitude
- **Part 2: Gathering Thai Restaurant data for each neighborhood from FoursquareAPI**: Get the venue data that belongs to the neighborhood and borough.
- **Part 3: Gathering additional information about the Thai Restaurant for each neighborhood from FoursquareAPI**: Get the additional venue data such as likes, ratings, and price.
- **Part 4: Gathering additional information about the Nearby Venues for each Thai Restaurant from FoursquareAPI**: Get the venue data that nearby Thai restaurants.
- **Part 5: Creating a new consolidated dataset of the IBM New York Dataset, along with their Thai restaurant, restaurant detail, and the nearby restaurants**: Merge all of the data frames into a single data frame for further analysis
