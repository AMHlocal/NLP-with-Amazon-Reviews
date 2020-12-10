# final-project

# Group - Cobra Kai
Members:
George Simon, Patrick Leon, Fred Mansfield, Austin Hauck

# Methodology

# Git Notes 
1. Before starting 'new' work: git checkout main
2. git pull origin main
3. git checkout yourBranchName
4. git merge main
5. git add .
6. git commit -m"detailed message"
7. git push
8. do your work
9. git add .
10. git commit -m"detailed message"
11. git push origin yourBranchName
12. Go to Github and make pull request. (Do this only when confident you want to update main repo)

# Making personal branch:
- clone repo to local
- nav to repo, type in: git checkout -b <your_branch>
- to switch branches: git checkout <branch_name>
- to upload to repo: git add . --> git commit -m "<descriptive message>" --> git push origin <your_branch>

# Write Up

## Back-End Development
______________________________
### DATA USED
* [Amazon Reviews - Link](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
    * Chosen Dataset: *amazon_reviews_us_Tools*
    * Note: for the purpose of this project we upload the data to our own Amazon s3 cloud storage.

### AMAZON S3
#### Requirements
* AWS Profile
​
#### Description
Utilizing Amazon AWS we choose to store our datasets in the cloud [S3](https://docs.aws.amazon.com/AmazonS3/latest/dev/Welcome.html) to access in our Googe Collab coding notebooks. Below is a link to the instruction readme for set-up and some notes on the free amazon services provided.
[Link to instructions.md](setup-instructions/amazon-S3-setup.md)

## Front-End Development
______________________________
### TABLEAU
#### Requirements
* Tableau Public Profile
    * [Tableau Public](https://public.tableau.com/en-us/s/)

#### Description
In order to set the stage and explore the Amazon Reviews Dataset Tableau Public was utlized.

Three vizzes were created to highlight different features of the data.
* Star Ratings Votes Over Time - *this chart also had Amazon's Stock Price overlayed*
* Votes Over Time
* Products with Helpful Reviews

All three of these vizzes can be found at the below Tableau Public link:
[Tableau Public Vizzes Link](https://public.tableau.com/views/Amazon_Review_Vis/StarRatingVotesOverTime?:language=en&:display_count=y&:origin=viz_share_link)
