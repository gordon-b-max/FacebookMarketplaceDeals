# Facebook Marketplace Analytics Project

## Description
Java project that takes an image of a product and outputs best deals on Amazon using the 
[Real-Time Lens Data API](https://rapidapi.com/letscrape-6bRBa3QguO5/api/real-time-lens-data/playground/endpoint_ea98df09-da49-42d7-bfe7-d45adcf189e7),
which interacts with the Google Lens API.

## Goals
Currently, right-clicking a static image on Google and selecting 'Search with Google Lens'
returns a selection of similar products or images matching the original image. 

1. Given a product on a resale website
(i.e. Facebook Marketplace), I want to return similar products that most closely match the 
original image on a verified e-commerce marketplace.

2. Based on the above response, rank the products by the best deals to compare against the resale product if it 
is a *good* or *bad* deal.
   
3. Create a Chrome extension or web application in the browser that checks if a resale product is a *good* or *bad* deal.


## Tasks
*GitHub tasks not based on priority or order to be assigned*

### Goal 1 
- Initialize Java Class that takes in a static `.png` or `.jpg` file and returns a list of related products 
- Create method that calls the [RapidAPI Real-Time Lens](https://rapidapi.com/letscrape-6bRBa3QguO5/api/real-time-lens-data/playground/endpoint_ea98df09-da49-42d7-bfe7-d45adcf189e7)
 from the `Product Google Lens API` with query param: `source=www.amazon.com`
- Create method that processes response from API call with a list of products by title and price
- Handle exceptions for API calls/responses if there is an issue with input image or returned products (i.e. no values returned or values for title/response)  
- Add unit tests during development w/ Mockito and JUnit tests




