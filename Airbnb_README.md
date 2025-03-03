# TripleTen Sprint 1 Project - Airbnb

### NYC Airbnb Data

This is the 1st project I worked on in the TripleTen Business Intelligence Analyst program. This project was the most fulfilling project I've worked on so far, and I loved it.

First I created separate sheet of the dataset to clean the data, then I create a copy of the raw data. Finally, I analyzed the data using pivot tables.

Taking the time to explain my results at each step was a key element in this process, and this was my first attempt at doing it. I wrote an introduction and conclusion that outlined what I did, and made suggestions for Airbnb to consider in the future.

### Data Usage

The data was spread across 3 sheets:

- `Data_Dictionary`: served as a reference document that provided detailed information about the data in the dataset. Its purpose is to ensure clarity, consistency, and proper data management by defining:
- Data Fields – Names, descriptions, and purposes of each field/column.
- Data Types – Specifies whether data is stored as text, numbers, dates, etc.
- Constraints – Defines rules, such as uniqueness, required fields, or relationships.
- Allowed Values – Lists possible values for categorical fields.
- Source & Lineage – Details where the data originates from and how it is processed.
- `Listings`: 65 rows each corresponding to unique key identifiers for NYC listings in the dataset
- id: Airbnb's unique identifier for the listing.  
- listing_url: URL of the listing on Airbnb.  
- scrape_id: Inside Airbnb "Scrape" this was part of.  
- last_scraped: UTC date and time this listing was "scraped."  
- source: Indicates whether the listing was found via "neighborhood search" or "previous scrape."  
- name: Name of the listing.  
- description: Detailed description of the listing.  
- neighborhood_overview: Host's description of the neighborhood.  
- picture_url: URL to the Airbnb-hosted regular-sized image for the listing.  
- host_id: Airbnb's unique identifier for the host/user.  
- host_url: The Airbnb page for the host.  
- host_name: Name of the host, usually just the first name(s).  
- host_since: The date the host/user registered on Airbnb.  
- host_location: The host's self-reported location.  
- host_about: Description about the host.  
- host_response_time: How quickly the host typically responds to inquiries.  
- host_response_rate: The percentage of messages a host responds to within 24 hours.  
- host_acceptance_rate: The rate at which a host accepts booking requests.  
- host_is_superhost: Indicates whether the host is a Superhost.  
- host_thumbnail_url: URL to the host's profile picture thumbnail.  
- host_picture_url: URL to the host’s profile picture.  
- host_neighborhood: The neighborhood where the host is located.  
- host_listings_count: The number of listings the host has (per Airbnb calculations).  
- host_total_listings_count: The total number of listings the host has across all locations.  
- host_verifications: Methods used to verify the host's identity (e.g., email, phone, government ID).  
- host_has_profile_pic: Whether the host has uploaded a profile picture.  
- host_identity_verified: Whether the host's identity has been verified by Airbnb.  
- neighborhood: The neighborhood as geocoded using latitude and longitude.  
- neighbourhood_group: A larger area that contains multiple neighborhoods, as geocoded.  
- latitude: The latitude of the listing's location (WGS84 projection).  
- longitude: The longitude of the listing's location (WGS84 projection).  
- property_type: Self-selected property type (e.g., apartment, house, hotel, bed & breakfast).  
- room_type: The category of the listing: Entire home/apt, Private room, or Shared room.  
- accommodates: The maximum capacity of the listing (number of guests).  
- bathrooms: The number of bathrooms in the listing.  
- bathrooms_text: A textual description of the number of bathrooms.  
- bedrooms: The number of bedrooms in the listing.  
- beds: The number of beds in the listing.  
- amenities: A list of amenities provided in the listing.  
- price: The daily price in the local currency.  
- minimum_nights: The minimum number of nights required to book the listing.  
- maximum_nights: The maximum number of nights a guest can stay.  
- minimum_minimum_nights: The smallest minimum night requirement from the calendar (over the next 365 days).  
- maximum_minimum_nights: The largest minimum night requirement from the calendar (over the next 365 days).  
- minimum_maximum_nights: The smallest maximum night requirement from the calendar (over the next 365 days).  
- maximum_maximum_nights: The largest maximum night requirement from the calendar (over the next 365 days).  
- minimum_nights_avg_ntm: The average minimum night requirement from the calendar (over the next 365 days).  
- maximum_nights_avg_ntm: The average maximum night requirement from the calendar (over the next 365 days).  
- calendar_updated: The last time the host updated the availability calendar.  
- calendar_last_scraped: The last time Airbnb’s system scraped the calendar data.  
- number_of_reviews: The total number of reviews for the listing.  
- number_of_reviews_ltm: The number of reviews the listing has received in the last 12 months.  
- number_of_reviews_l30d: The number of reviews the listing has received in the last 30 days.  
- first_review: The date of the first/oldest review.  
- last_review: The date of the most recent review.  
- review_scores_rating: The overall rating score based on guest reviews.  
- review_scores_accuracy: Rating score based on how accurate the listing description is.  
- review_scores_cleanliness: Rating score based on the cleanliness of the listing.  
- review_scores_checkin: Rating score based on ease of check-in.  
- review_scores_communication: Rating score based on the host’s responsiveness and communication.  
- review_scores_location: Rating score based on the location of the listing.  
- review_scores_value: Rating score based on the value for money.  
- license: The listing's permit, license, or registration number (if applicable).  
- instant_bookable: Whether guests can book instantly without host approval (true/false).  
- reviews_per_month: The average number of reviews per month over the lifetime of the listing.  
- `Calender`: Analysis on how much money each listing generated over the timespan of one year. 
- listing_id: ID number that uniquely identifies each property	
- date: representing the date the rental was first rented 	
- available: the availability of each rental using (t) or (f)
- price: of rental property 
- adjusted_price: represented price adjustment for each day a property is rented	
- minimum_nights: representing minimum nights rented per property 	
- maximum_nights: representing maximum nights rented per property
- revenue_earned: representing the revenue earned each night

The data is provided by TripleTen

### The Process

I sourced data from the "Listing" and "Calendar" sheets to analyze Airbnb property attractiveness based on reviews from the past 12 months, using **number_of_reviews_ltm** as the key metric. I created pivot tables to identify the top 10 neighborhoods and the most popular property sizes, then recommended specific sizes for each neighborhood. Finally, I estimated annual earnings for these listings by multiplying 30-day revenue by 12 and added a column for **"estimated_earnings"** to show potential yearly income.

### Results
Taking the time to explain my results was a key element in this process, and this was my first attempt at doing it. I wrote an Executive Summery and Assumption that outlined what I did.

Please have a look at the Google Doc Spreadsheet included for a full description of the results.
