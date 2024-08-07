# Merry Christmas All Around the World

![Data](https://github.com/Arpita-deb/How-to-say-merry-christmas-in-different-languages/assets/139372731/44903ac1-6b02-40db-bfd9-dad6645768a0)

## Introduction: 

This repository contains the documentation of my dashboard creation process as a part of the Romanian Data Tribe Challenge for 2023. I’ve enriched the data from the challenge, which mainly covers European countries, with external data from other regions of the world. With this data, I’ve designed a dashboard that displays the different ways of saying Merry Christmas across the globe, using Tableau and Canva.

## About the Challenge:

The competition is held by [Romanian Data Tribe Challenge for 2023](https://data.world/romanian-data/merry-christmas-in-european-languages). The challenge is to "Create a beautiful visualization for the data attached (you may use extra datasets too)". The ranking for the 1st place will be based on a weighted average of votes (30% importance for Public Votes, 70% of importance for Co-Leaders Votes)

**Deadline**: December 20, 2023

## Data Source:

[Romanian Data Tribe Challenge for 2023](https://data.world/romanian-data/merry-christmas-in-european-languages)

## External Data Used:

* [How to say "Merry Christmas" in all languages in 2023](https://polyglotclub.com/wiki/Language/Multiple-languages/Vocabulary/Merry-Christmas-in-all-countries-languages)
* [List of official languages by country and territory](https://en.wikipedia.org/wiki/List_of_official_languages_by_country_and_territory#:~:text=List%20of%20countries%2Fterritories%20%20%20%20Country%2FRegion%20,%20%20%20%2023%20more%20rows%20)

## Tools used:

1. Tableau - To create the dashboard
2. Canva - To add the title in the dashboard
3. Excel -  For cleaning the data

## Data Cleaning:

1. Created a back-up copy of the original dataset _merry_chrsistmas_in_european_languages_.
2. The _merry_chrsistmas_in_european_languages_ dataset contains 3 columns - _country, language_ and _how to say "merry christmas"_. The information present is from European countries only.
3. To make it complete, I added external data from various reliable sources to create a global dashboard with countries from different continents.
4. In order to do that I created a different excel spreadsheet where I dumped all the data from [How to say "Merry Christmas" in all languages in 2023](https://polyglotclub.com/wiki/Language/Multiple-languages/Vocabulary/Merry-Christmas-in-all-countries-languages) and named it _country_merry_xmas_.
5. The data in _country_merry_xmas_ consists of 2 columns - _country_ and _how to say "merry christmas"_. In order to map these data points with the official/spoken language I have to collect data with countries and their respective official languages.
6. To do that, I created another sheet in the excel spreadsheet and called it _country_language_. Here I dumped a table from [List of official languages by country and territory - Wikipedia](https://en.wikipedia.org/wiki/List_of_official_languages_by_country_and_territory#:~:text=List%20of%20countries%2Fterritories%20%20%20%20Country%2FRegion%20,%20%20%20%2023%20more%20rows%20) and removed the redundant columns. I ended up with 2 columns country and official language.
7. I cleaned this sheet by removing the [] from the end of the country and language columns, removed the formatting, trimmed for white spaces and changed the cases. 
8. Now, I have 3 excel sheets, the original dataset _merry_chrsistmas_in_european_languages_, _country_merry_xmas_ with data from all continents and _country_language_ with data regarding country and official language. To create a coherent,comprehensive and complete dataset, I have to join these three datasets.
9. In this step, I filtered for the countries in _country_language_ sheet for the countries present in _country_merry_xmas_ sheet, in order to fill up the language column in _country_merry_xmas_ sheet.
10. Then I manually joined _country_merry_xmas_ and _country_language_ sheets.
11. I ended up with 2 sheets, the original _merry_chrsistmas_in_european_languages_ sheet containing data from only European countries and _country_merry_xmas_, containing data from all over the world including some european countries as well.
12. Next, I joined these 2 spreadsheets by copy and pasting the data from _merry_chrsistmas_in_european_languages_ sheet to _country_merry_xmas_ sheet.
13. By joining these tables together, I ended up with a few duplicate entries. I removed these duplicates by using Remove Duplicate from the menu.
14. Now, I have one spreadsheet with data from 3 different datasets.
15. In this step I started data cleaning of the final dataset. I changed the cases of the columns to Proper case and trimmed for leading and trailing spaces from all the columns.
16. I've added English pronunciations to _how to say "merry christmas"_ columns for some languages.
17. Finally saved the data as _how_to_say_merry_christmas_in_many_languages_, which is used to create the dashboard


## About the Dashboard:

![christmas](https://github.com/user-attachments/assets/774918f2-1ee1-4661-9834-41104553c539)

The dashboard is created using Tableau and Canva. This contains a simple global map, with country name and how to say Merry Christmas in that country as Labels. When hovered over any country, the tool tip shows these information: country,continent, language and how to say Merry Christmas in that language. The dashboard contains a title as well as additional information regarding the challenge.

## Resources:

* [Link to the dashboard](https://public.tableau.com/views/HowToSayMerryChristmasInManyLanguages/MerryChristmas?:language=en-US&:display_count=n&:origin=viz_share_link)
* [Image in the dashboard](https://unsplash.com/photos/two-elf-on-the-shelf-figurines-kFbSKhukfIQ)
* [How to say Merry Christmas in different European Languages Original Dashboard by Jakub Marian](https://geographyeducation.org/2015/12/18/how-to-say-merry-christmas-in-different-european-languages/)
* [How to Say Merry Christmas in 21 Different Languages](https://www.mondly.com/blog/how-to-say-merry-christmas-different-languages/)
* [HOW TO SAY MERRY CHRISTMAS IN 25 DIFFERENT LANGUAGES – INCLUDING KLINGON!](https://blog.pimsleur.com/2018/12/20/merry-christmas-in-25-languages/)
* [How to say happy holidays & Merry Christmas in 106 languages](https://www.berlitz.com/blog/merry-christmas-different-languages)

