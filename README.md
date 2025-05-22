# Final-Project-Tableau

## Project/Goals
The scope of this project was to show familiarity and proficient ability in working with Tableau and a given data set to graphically present meaningful correlations between the data. This was done by connecting the data set to Tableau and then detecting keypoints to start building the visualizations with, and to create a dashboard that would answer self-defined questions to ask of the dataset. OPTION 2.3 was chosen for this project. Wherein Airbnb data of listings in NYC from "Inside Airbnb" was taken to create a dashboard. (The data file used can be found in the Data directory under [airbnb_data_cleaned.xlsx]().)

## Process
### Step 1:
Some initial assumptions were made in preparation to interpret the data. Namely that the "Prices" data listed in the dataset are PER NIGHT, and that the "Host Since" data listed also represents the initial date that the associated listing was put into service.

Additionally, the data in the provided spreadsheet was cleaned prior to being connected to in Tableau. This was done by filtering out the entries with Null values to streamline and make consistent the entries in the dataset. Null values were found in the following data:
-   Host ID
-   Price
-   Zip Code
-   (No. of) Beds (Not having beds made it an irrelevant listing as the context for Airbnbs is a place to stay)
-   Reviews (Not having reviews is captured as "0" reviews, null is suspect)
-   All listings with null/empty review scores but have reviews (No. of Reviews) as ratings are required with submitted reviews
-   Listings with suspect names (There was one named "Let's make a deal..." as a shared room for $2500/night, and one named "NO LONGER BOOKING RESERVATIONS" listed at $10,000/night)

Once this was done, the data could loaded/connected to within Tableau.

### Step 2:
Once in Tableau, the data was analyzed to verify the different types that were present. A mixture of strings, integer values, date values, and geographic values were found. They all corresponded intuitively to the type of data presented.

Additionally, a second round of filtering within Tableau was performed to further streamline and make consistent the data to be interpreted. For example, while valid line entires, the listings with zip codes outside of NYC were filtered out, as this dataset was meant to focus on listings within NYC. Zip codes for locations in Washington state, California, Massachusetts, and New Jersey were ommitted.

### Step 3:
At this point - with the data verified, cleaned, and filtered - visualizations were built according to the data's categorical features. Relationships with meaningful information that could be gleaned were used to generate graphical representations of their correlations.

### Step 4:
With the visualizations (Tableau Worksheets) created, their conveyed informative results were considered to apply to different questions that they could answer. These were pondered and informed the formation of the Dashboard that would be created using these Worksheets.

### Step 5:
A presentation is then preapred using this information, with the intention to convey the functionality of this dashboard. The information which was interpreted from this graphical representation of the data will be documented in said presentation.

## Results
As Option 2.3 - Airbnb dataset was selected, the visualizations that were created mainly pertained to location, cost, and listing reviews. The overarching question was whether there were any correlations between the host, the location, and the amenities (beds, room type, property type, cost) with the review ratings. The result Dashboard can be found in the Tableau Workbook directory under [JN_airbnbNYC_Proj.twbx]().

The first graphic was a map of New York City, with each listing location based on Zip Code (as no specific coordinates or addresses of each property were provided/available) represented. Categorical filters such as the Neighbourhood they were in, the types of rooms offered, number of beds, and average cost per night were also applied to allow for a flexible viewing experience. This map would provide summarized info on the listings in the area with specifics listed on a Tooltip when hovering a cursor over the location dot.

The second visualization was a side-by-side bar graph to show the average price per night of each room type within each neighbourhood. This format was selected to better compare at a glance what the pricing trends may be, as impacted by these 3 factors.

The third visualization was a scatter plot comparing the hosts' tenure as Airbnb hosts with their reviews (both number of, and review scores). This was to try to glean a trend as to whether longer tenured hosts would have more, and higher rated, reviews. A trendline was included to better gauge what the overall conclusion would be. A colour-range was used to denote the ratings from each review.

The fourth visualization was an animated historical timeline superimposed onto a map of the NYC area. This was to show the number of Airbnb listings that have been put into service over time. At a glance, this can easily tell which areas, zip code locations, and room types became more popular to host, over time.

The fifth visualization was a cluster scatter plot. This made use of the clustering technique for listings to better categorize the "tiers" of the Airbnb rooms. It clustered number of beds, price, and review scores to compare with the average price per night to graphically show correlations to the factors that may impact the popularity and the price.

The result was that there seemed to be quite a bit of correlation between the host, the location, and the amenities (beds, room type, property type, cost) with the review ratings, as hypothesized. It can be easily represented and with the generated visualizations, and would cater to a wide range of audiences, depending on how it is conveyed.

## Challenges 
The main challenge with this project was becoming familiar with Tableau's capabilities and making use of it to answer the questions that its graphics would be best suited to do so. The UI of Tableau makes sense but is not immediately intuitive due to the sheer scope of the capabilities that it holds as a graphical data representation tool.

## Future Goals
If there was more time, I would use it to experiment more with Tableau, to see what other ways its features can be combined and used in tandem to represent more robust, flexible, and nuanced visualizations. Additionally, while the visualizations looked presentable, I would like to explore how best to tweak the representations beyond the defaults to really tailor the graphical theming to a specific audience.
