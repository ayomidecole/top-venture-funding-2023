# top-venture-funding-2023
A quick analysis of a Kaggle [dataset](https://www.kaggle.com/datasets/adnananam/largest-us-venture-funding-deals-of-2023?resource=download) with the 171 top venture funding rounds in 2023

I wrote an article on my new publication On Data and Stories. You can read the article [here](https://www.linkedin.com/pulse/top-venture-deals-2023-ayomide-aremu-cole-5xmye/?trackingId=jJpZOOyHQJGlTq5OKTgMqw%3D%3D)

## Methodology
_This might not follow the order of operations in the Jupyter Notebook but this is how I approached the problem_

1. I examined the dataset to see what it was about.
2. I wanted to know which indusry had the most funding rounds in the dataset, so I created a pivot table showing the count by industry. BioTech funding rounds lead the pack followed by AI.
3. I also created a bar chart to visualize the top 5 industries by funding rounds.
4. I wanted to dig deeper into this and compare the funding rounds for Biotech and AI. I checked the datatype for the funding amount (amount) column, the column was an object datatype so I converted it to float so that I could run numerical operations.
5. The funding rounds were mostly in millions and billions so to make the data easier to interact with, I converted them all to billions by dividing the column by 10^9.
6. With this I could calculate which industry had the most money come in. I separated Biotech and AI funding rounds into 2 dataframes to complete this analysis.
7. I found that even though there were more BioTech deals done. AI brought in more funding dollars than Biotech which tracks with the AI hype cycle.

Enjoy and feel free to mess with the data yourself and see if you find different insights.
