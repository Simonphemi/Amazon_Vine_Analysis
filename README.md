# Amazon_Vine_Analysis
This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members. For the first part of the project, created a cloud relational database using Amazon Web Services (AWS) and connected our database using a PostgreSQL. We then created four tables in our RDS using the schema provided. Finally, we extracted Amazon review dataset regarding video game reviews, transformed the data based on the directions provided for the Challenge and then uploaded the data into our cloud database tables. We used postgreSQL to create our tables and PySpark for the ETL process.

# Amazon_Game_Review_Analysis
For the second deliverable, we again extracted video game Amazon review datasets and loaded the data into a new GoogleColab notebook using PySpark. We filtered the data to only include games where total reviews received were greater than 20. We then further filtered the data to include games where the proportion of helpful votes to total is greater than or equal to 50%. Finally we divded the dataset into two groups: reviews given as part of the vine program(paid) and reviews given oustide the vide program(unpaid). Using the two datasets, we compared the ratio of proportion of 5-star reviews to total reviews between reviews obtain from the vine program and reviews outside the vine program. Our Analysis Code for this exercise is also included in this repository.

## Results
When comparing 5-star ratings between the two datasets, we noted that the proportion of 5-star ratings in the Vine program is around 51% while the proportion of 5-star ratings in reviews outside the vine program drops to 38.7%. 
Screen Shot 2021-06-21 at 3.35.49 PM<img width="614" alt="Screen Shot 2021-06-21 at 3 35 49 PM" src="https://user-images.githubusercontent.com/79813670/122817942-9029e180-d2a6-11eb-9029-8bef6d7d6c43.png">
Screen Shot 2021-06-21 at 3.36.05 PM<img width="764" alt="Screen Shot 2021-06-21 at 3 36 05 PM" src="https://user-images.githubusercontent.com/79813670/122817982-9ddf6700-d2a6-11eb-8dd8-3d9212bee75f.png">
# Summary
As we can see, there is a significant increase in 5-star reviews (almost 12%) when reivews are obtained from the Vine Program. This suggests a positive bias for reviews within the vine program.

We could however perform further analysis into this data. We could compare the proportion of all the ratings instead of only focusing on 5-star ratings. We could then provide a better picture on whether a bias exists accross all ratings and not just the top rating. We could also compare the average rating within the two data sets (vine and not vine) to determine if there is a general probability of reviewers providing better reviews within the vine program.
