# EDA-DC and Marvel Comic Character
This is a Exploratory Data Analysis of the DC - Marvel Comic Character dataset.

This public dataset was obtained from Kaggle [Dataset DC-Marvel Comic Characters](https://www.kaggle.com/datasets/nikhil1e9/comic-characters)
thanks to NIKHIL 

The dataset consists of several features, such as:
1. Name: The name of the character
2. Identity: The identity status of the character (Secret Identity, Public identity, etc.)
3. Alignment: If the character is Good, Bad, or Neutral
4. Eyes: Eye color of the character
5. Hair: Hair color of the character
6. Sex: Sex of the character (e.g. Male, Female, etc.)
7. Alive: If the character is alive or not
8. Appearances: The number of appearances of the character in the comics
9. First_appeared: The month and year of the character's first appearance in a comic book
10. Planet: The planet to which the character belongs
11. Universe: Which of the two DC or Marvel universe the character belongs to

## Here are the results
### Conclusion EDA DC-MARVEL CHARACTER
1. The columns in the dataset are mostly of object type and only 2 are of Int type.
2. The dataset does not contain missing values, but there is a column First_appear which is an object type while it should be a DateTime data type so a data type conversion is done first. And there is a date with the name Holiday, because there is no Holiday month name, here I drop it.
3. After converting First_appear and separating the columns by month and year, there are 136 missing values in the Month column. Because the missing value is below 1%, I drop the missing value data.
4. From the correlation heatmap, it can be seen that the correlation between numerical columns is weak so it is concluded that there is no strong influence between the Id, First_appear, and Appearances columns.
5. In the Barplot, it can be seen that the distribution of characters is most prevalent in the Marvel Universe compared to DC.
6. It can be seen in the boxplot and scatterplot in the 2 Universes that the gender of the characters is mostly male with the majority of blue eye color and black hair
7. In the Barplot, it can be seen that the 2 Universes have more characters who are alive than dead
8. In the Barplot, it can be seen that the character's identity in the Marvel Universe is mostly Secret while DC's secret and public identities are almost equal
9. The Boxplot shows the possibility of outliers because there are characters that appear above 1000 times.
10. In the Appearances vs First Appear Scatterplot, the distribution of data is mostly scattered mostly below 500 so it can be concluded that the characters appear on average no more than above 500 times.

### Insight
From the dataset, it is known that the Marvel Universe has more characters than the DC Universe. From both Universes, the characters are dominated by the male gender with the characteristics of blue eyes and black hair and the average appearance of the character from the first time it appears is approximately 500 times. The character traits in the Marvel Universe are dominated by bad characters, inversely proportional to the DC Universe where good characters are slightly more than bad characters.
