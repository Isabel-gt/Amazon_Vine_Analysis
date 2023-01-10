# Amazon_Vine_Analysis

## Overview of the Project
<p align="justify">The purpose of this project was to analyze the Amazon reviews written by members of the paid Amazon Vine program. “The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.” (bootcampspot, 2023)</p>
<p align="justify">The dataset chosen to perform the analysis was picked randomly from 50 Amazon review datasets. The one selected for the analysis was one that contained book reviews.</p> 
<p align="justify">Using PySpark an ETL (Extract, Transform, Load) process was performed. The data was connected to an AWS RDS (Amazon Relational Database Service) and it was loaded to pgAdmin.</p>  
<p align="justify">There was a second objective of the project. The other goal was to determine if there was any bias toward favorable reviews from Vine members in the dataset. This part of the project was done using PySpark in Google Colab.</p> 

## Results
The dataset used in the first part of the analysis was used for the second part as well. Unfortunately, that dataset did not include any Vine program reviews. 

<img width="703" alt="0" src="https://user-images.githubusercontent.com/111388644/211665545-a1c2b9c6-5dec-42cd-b728-e1774119c010.png">

<img width="369" alt="0 1" src="https://user-images.githubusercontent.com/111388644/211665583-7b048831-50e4-48c1-a1ca-7fe9cfdfcb7d.png">

Because of this, answering the questions was not going to lead to any conclusions. 

<img width="657" alt="0 2" src="https://user-images.githubusercontent.com/111388644/211665610-0ac6a7c9-da47-4aeb-b835-6ff2ac8afd48.png">

Therefore, another book dataset chosen from the same 50 Amazon review datasets. With this second data set the analysis was performed, and the following questions were answered:
 
•	How many Vine reviews and non-Vine reviews were there?
In the case of the second book dataset, there were 4781 reviews of the Vine program (paid). On the other hand, there were 332395 reviews of the unpaid option. This is displayed in the images below:


<img width="347" alt="1" src="https://user-images.githubusercontent.com/111388644/211665641-83bdcbc7-fbd3-40b6-bfce-22c01d9d8211.png">


<img width="287" alt="2" src="https://user-images.githubusercontent.com/111388644/211665675-5987bc6e-5bf1-4532-86c9-61b26c5c81f2.png">


•	How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
There were 1604 Vine reviews that had a 5-star rating. These number of reviews are smaller compared to the unpaid ones that were 168800.

<img width="611" alt="3" src="https://user-images.githubusercontent.com/111388644/211665720-73947e21-f623-4e9a-8ebd-6cdc5f65dd4c.png">


•	What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
The percentage of the Vine reviews (paid program) was 33%. Because there were more revies of the non-Vine program it is expected that the percentage of 5-star reviews is higher in this program as well. The percentage of non-Vine reviews (unpaid) that had a 5-star rating was 50%.

<img width="442" alt="4" src="https://user-images.githubusercontent.com/111388644/211665788-7f5eb592-0451-4484-aaf5-d847fcaa2d85.png">


## Summary
<p align="justify">In the case of the first dataset there were no paid reviews. In other words, the reviews that were supposed to come from the Vine program were not existent. This gives little to no room to make conclusions about the vine program.</p> 

<p align="justify">Although those conclusions are not possible to make, it is clear that there were a lot of 5-star reviews (60%). This indicates that the overall satisfaction with the books is a positive one.</p>

<p align="justify">To get insight regarding the Vine program the analysis should be performed on a different data set.</p> 

<p align="justify">The analysis was performed in a second dataset, that was also of book reviews.</p> 

<p align="justify">There seems to be no positive bias when it comes to the reviews in the Vine program since there is only 33% of 5-star reviews. If there was a bias this percentage would be expected to be higher.</p> 

<p align="justify">Also, the percentage of 5-star rating of the non-paid reviews is 60%, which means that overall, there is a lot of satisfaction of the product (books). This could help to argue against the people that might think the percentage of 5-star reviews of the Vine program is too high.</p>
