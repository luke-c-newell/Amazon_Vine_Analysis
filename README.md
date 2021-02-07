# Amazon_Vine_Analysis
## Overview
In this repository, I have used the PySpark library in Google Colab, an AWS RDS database and PostgreSQL to create an ETL process for analyzing Amazon reviews. My client is interested in analyzing whether there is any bias in reviews completed as part of the Amazon Vine paid review program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review of the product.

Using a Jupyter Notebook and the Pandas library, I have analyzed the reviews in the US Lawn and Garden category, to determine whether there is any bias between 5 star paid Vine reviews and 5 star unpaid reviews. To ensure accurate results, I have filtered the dataset to only include reviews where there are more than 20 total votes and where the percentage of helpful reviews was over 50%.

## Results
#### Vine reviews DataFrame
![vine_reviews](https://github.com/luke-c-newell/Amazon_Vine_Analysis/blob/main/images/vine_reviews.png "vine_reviews.png")

#### Non-Vine reviews DataFrame
![non_vine_reviews](https://github.com/luke-c-newell/Amazon_Vine_Analysis/blob/main/images/non_vine_reviews.png "non_vine_reviews.png")

### How many Vine reviews and non-Vine reviews were there?
- Vine reviews - 386
- Non-Vine reviews - 48717

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- Vine reviews - 176
- Non-Vine reviews - 24026

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- Vine reviews - 45.6%
- Non-Vine reviews - 49.3%

## Summary
### Is there any positivity bias in the Amazon Vine program?
Overall, the results show that there is no positivity bias for Amazon Vine reviews in the Lawn and Garden category. This is supported by the results as fewer Vine reviews gave 5 stars (45.6%) when compared to helpful reviews from non-Vine reviewers (49.3%). This suggests that Amazon Vine reviewers may be more critical of the products they review than the general population of Amazon reviewers.

### Additional Analysis
To further understand whether paid Amazon Vine reviews show any positivity bias, I could repeat the analysis on another category of Amazon reviews. Amazon Vine reviewers in the Lawn and Garden category may not show the same bias as reviewers in another category, which would allow me to understand if this trend continues across different products.
