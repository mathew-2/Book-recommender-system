# Book-recommender-system


This is a Book recommendor system that uses a collabrative-filter based learning system to suggest familiar books based on user input 

## The concept

This project is in itself two parts.
The first part is the home page where the top 50 books having top ratings and are read by many people are displayed for the user to review

The second part is the recommend page where based on the user suggestion given, the books suggested by "intellectual users" meaning users that have read alot of books and the books having more than 250 ratings are taken.Then the ratings given by users will be represented as a vector ,where according to **each book** the ratings given by these **intellectual** users will be **one vector**.Then according to the Book given by user input the  5 vectors closest to the vector of the book given will be suggest  

Here the dataset used is an old dataset,but based on really famous books
