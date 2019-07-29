# AppProfileRecommendation

You can download the data set from the link below:<br>
https://www.kaggle.com/lava18/google-play-store-apps/home<br>
https://www.kaggle.com/ramamet4/app-store-apple-data-set-10k-apps/home<br>

Project Synopsis: Data Analysis for a company that builds Android and iOS mobile apps. All the apps build by this company is free and 
the main source of income is in-app ads. That means the revenue for any given app is mostly influneced by the number of users who use 
the app- the more the users that see and engage with the ads, the better.<br>

Conclusion:
In this project we started exploring the dataset. After exploaration we found that dataset is not perfect for ananlysis. It has missing values, duplicate entries, non english apps and non free apps. We started with removing the rows which has missing values in their coulmns. After that we removed the duplicate apps. We gave the preference to the maximum number of reviews. We kept the app app which has the maximum number og reviews and deleted rest of the rows including the same app name. We created a dictionary with the unique app names and built a new data set using this dictionary.
After that is done we removed the non english apps with the help of ord() function. Our approch was as follows if the value return by the function ord() is greater than 127 than it is not an English alphabet. But it leads to remove lot of rows which were having some special character in theie app name column. To fix this issue we kept this critiera, if an app name has more than 3 non english characters then only consider it as an non english app. We further refine the data set on the basis of its cost.
After all this done we then moved towards the data analysation phase. In which we made a frequecy table on the basis of Genre of the app. And later we made a table in which we added all the genres with their average number of installs.
At conclusion, we can suggest our company to make app in Book genre. It does not requires any external resources such as subscription from any other source. There are lot of good books are available in the market. They only need to find a good book. They can add features like dictionary, daily quotes from that book etc. This could be great app for both android and ios platform.

Thank you
