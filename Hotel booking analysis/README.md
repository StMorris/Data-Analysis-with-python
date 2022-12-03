# Hotel Booking Analysis

The dataset contains data from two different hotels. One Resort hotel and one City hotel. From the publication (https://www.sciencedirect.com/science/article/pii/S2352340918315191) we know that both hotels are located in Portugal (southern Europe), One of the hotels (H1) is a resort hotel in Algarve and the other is a city hotel (H2) in Lisbon. The distance between these two locations is ca. 280 km by car and both locations border on the north atlantic.

Each observation represents a hotel booking. The datasets contain bookings due to arrive between the 1st of July of 2015 and the 31st of August 2017, including bookings that effectively arrived and bookings that were canceled. For my analysis i will only use bookings that were not cancelled, to get actual guests numbers that were recieved.

#### Questions?
- Where are the guests from?
     - Spatial analysis on the location the guests are from
- How much do guests pay for a room per night?
- How does the price per night vary over the year?
- Which are the most busy month?
- How long do people stay at the hotels?
- Bookings by market segment
- How many bookings were canceled?
- Which month has the highest number of cancelations?
- Why are prices for aviation so high?


kindly paste notebook link here  (https://nbviewer.jupyter.org) to view plotly interactive visualization


### Results

#### People from all over the world stay in these two hotels. Most guests are from Portugal and other countries in Europe
<img src = "https://github.com/StMorris/Data-Analysis-with-python/blob/main/Hotel%20booking%20analysis/guests_location.png"
     style = "width:800px;height:500px"/>


##### Prices in the Resort hotel are much higher during the summer (june 1- august 31),while prices in the city varies less and is most expensive during spring (march 1 - may 31) and autumn (september 1 - november 30).   

<img src = "https://github.com/StMorris/Data-Analysis-with-python/blob/main/Hotel%20booking%20analysis/room_price_pernight_month.png"
     style = "width:800px;height:500px"/>
     
<img src = "https://github.com/StMorris/Data-Analysis-with-python/blob/main/Hotel%20booking%20analysis/avgnum_guests_month.png"
     style = "width:800px;height:500px"/>

#### On the average Groups get the best prices while aviation gets the highest prices. AVD(AVerage Daily Rate)
<img src = "https://github.com/StMorris/Data-Analysis-with-python/blob/main/Hotel%20booking%20analysis/ADR_market_segment.png"
     style = "width:800px;height:500px"/>
     


##### Why are the prices for aviation so high? - open the notebook to experience the analysis on Paid App Prices by Category
