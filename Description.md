<center><h1>Coursera Capstone</h1>

<h2>IBM Applied Data Science Capstone</h2>
</center>

<center>Opening a New Fitness Club in Moscow, Russia<br/>
By: Alexander Konnov<br/>
April, 2021
</center>


<h3>Introduction</h3>

This project focuses on the selection of the optimal location for a fitness club in Moscow, Russia.

The review [Forbes](https://www.forbes.ru/biznes/417589-razrushitelnoe-cunami-2020-god-stal-hudshim-za-vsyu-istoriyu-rossiyskoy-industrii) claims that during the pandemic, about 60% of market participants were broken.

Currently, restrictions on visits to offices, shops and entertainment centers, which include fitness clubs, are gradually being lifted. New players are expected to emerge, as well as the return of old customers.

**Business problem**

It is necessary to assess the prospects of certain districts of Moscow in terms of placing new fitness clubs there. Using Data Science and clustering methods, it is necessary to prepare answers to the question of where is the most profitable to open a new fitness club.

The report should provide answers to the following questions:

- The most efficient location for a fitness club aimed at office workers

- The most efficient location for a family oriented fitness club.


**Target of this project**

The target audience of this project are investors, as well as large networks of fitness centers that want to effectively use their funds in the context of economic recovery.

<h3>Data</h3>

**Data to solve the problem**

Data expected to be used in preparing this project:

1. List of administrative districts of Moscow, Russia
2. Geocoordinates of individual administrative districts
3. Venue data, particularly data related to fitness clubs. We will use this data to perform clustering on the divisions


**Data sources and methods to analyze**

A list of all administrative districts of Moscow is available at the link [https://en.wikipedia.org/wiki/Template:Administrative_divisions_of_Moscow]

The Web scraping technique is used to extract information using Python and the BeautifulSoup package.

Wikipedia is also used to obtain the geographic coordinates of the location of each district. Geographic coordinates are indicated on the pages of individual districts. It was decided to refuse to use the Geocoder package, as it does not work reliably.

After that, we will use Foursquare API to get the venue data for those divisions. Foursquare has one of the largest database of 105+ million places. Foursquare API will provide many categories of the venue data, we are particularly interested in the Sports category in order to help us to solve the business problem put forward. This is a project that will make use of many data science skills, from web scraping (Wikipedia), working with API (Foursquare), data cleaning, data wrangling, to machine learning (K-means clustering) and map visualization (Folium).
