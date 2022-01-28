   <center><img width="594" alt="Screen Shot 2022-01-28 at 4 02 09 AM" src="https://user-images.githubusercontent.com/92389914/151527350-ff17c06d-6630-47f4-90e8-e228af2a9c47.png"></center>

# Kaylees new toy: Using Amazon data to recommend a new toy for my daughter
Author: Deja Prade

# Overview

In this project, I build a toy recommendation system using the amazon e-commerce data. I develop a content-based recommendation model using NLP and cosine similarity and a collaborative-based model using SVD. 

# Business Understanding

Kaylee (my stakeholder/daughter) is a one year old whom is pretty spoiled. Of course we do things the old-fashion way and pick out random toys in local stores but since starting the Flatiron Data Science program I haven't had much time for that. I wanted to develop a toy recommendation system to balance out school and mom life.

# Data

[Data](https://www.kaggle.com/PromptCloudHQ/toy-products-on-amazon)

I used toy data from Amazon E-commerce which includes 10000 products. The dataset contains product names, ids, catergories, average ratings, description and etc.

# Model

To build my recommendation system I used a content based system which relied heavily on review text  and a collaborative based system using product average ratings. Content-based and collaborative filtering are two of the most common types of recommendation systems. I did my recommendations based off of the toy “Disney dancing plush doll series Minnie mouse” because Kaylee loves Minnie Mouse. 

<img width="816" alt="Screen Shot 2022-01-26 at 2 21 06 PM" src="https://user-images.githubusercontent.com/92389914/151525732-194c0c4a-f754-4589-9279-bbf86559036d.png">

### Content based filtering

For my content based modeling I used cosine similarity which measures the how similar two product names are. I used the columns product name (which was my target description of product, category and customer reviews. 

<img width="309" alt="Screen Shot 2022-01-28 at 3 28 23 AM" src="https://user-images.githubusercontent.com/92389914/151525911-dab7f0e1-a59d-4896-9c10-77fbef5ba388.png">

### Collaborative based filtering

For my collaborative based model I used Singular Value Decomposition aka SVD. The SVD of a matrix is a factorization of that matrix into three matrices. I use the columns product name (again as the target), unique ID, price, and average review rating. 

<img width="386" alt="Screen Shot 2022-01-28 at 3 25 18 AM" src="https://user-images.githubusercontent.com/92389914/151526097-b8d09460-c19a-4ab2-ae6f-a1a336e29a82.png">

# Conclusion

The recommendation systems are favorable. Each list contains toys Kaylee would actually play with or already owns one similar. When shown pictures of the toys she pointed out multiple she was attracted to.

### Next steps

My next steps to improve this project would be to find data to merge with this dataset that contains information about individual users so that I can build another collaborative model. I could also dive deeper to recommend toys based on toys previously viewed. Lastly I would build a hybrid model to compare then build a streamlit app.
