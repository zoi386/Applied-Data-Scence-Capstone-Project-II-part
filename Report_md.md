
<h1 align = center><font size = 6>APPLIED DATA SCIENCE CAPSTONE PROJECT</font></h1>
<h3 align = center>(WEEK 1)</h3>


<h1 align = center>Record of Protected Structures</h1>
<h2 align = center>Galway County Ireland</h2>

Data:
[Published by: Galway County Council](https://data.gov.ie/organization/galway-county-council)
[Licensed under: Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)

### Introduction 
A protected structure is a structure that the Planning Authority considers to be of special interest from an architectural, historical, archaeological, artistic, cultural, scientific, social or technical point of view. The Planning Authority in its Record of Protected Structures (RPS) includes details of protected structures.A Record of Protected Structures is the record included in a Development Plan, correct at the time of publication. It may be amended by the addition or deletion of entries independently of the Development Plan review process.[source](https://data.gov.ie/dataset/record-of-protected-structures1/resource/de1217cb-5c97-434c-8b05-2114967f642c)

As it was clearly stated in first paragraph **'Protected structures' are considered to be of special interest** for local goverment and comunity. They have architectural, historical, archeological, artistic, cultural, scientific, social or technical value. These structures in futher text I will call *Cultural heritages*. 
According to [WIKIPEDIA](https://en.wikipedia.org/wiki/Cultural_heritage)  '*Cultural heritage* is the legacy of physical artifacts and intangible attributes of a group or society that is inherited from past generations. Not all legacies of past generations are "heritage", rather heritage is a product of selection by society.'

As such these Structeres does not just represent rich history and cultural achievements of one nation, group of people or single person, they also inform us about lot of aspects of life from one time, interconnectivity, influence from other nations, struggle one been through. They are keepers of one nation past and history but also enrichment for others.
In todays societies in time of globalisation, will of one to get know better others is highly valuated. These needs 'to get know and see others',  that are common to all human beings, are primarly satisfied through traveling. **Tourism** is highly appreciated brunch of industry of any country. It brings ravenue but is also beneficial for other industries such as agriculture, small local retail shops, hotels, restaurants museums and other so called tertiary activities. 
It has its bad sides as well, such as overcrowding, waste and noise and it should be addressed properly by responible such as Tourist agencies and domestic governments in order to minimase these negative impacts on local comunities as well as tourists. 


**Ireland** is beautiful green island in the North Atlantic Ocean. It is divided on Republic of Ireland and Northern Ireland which is part of United Kingdom. It is noted for a rich cultural heritage and tradition that is mainly linked to Gaelic language. Ireland is home for 6.4 million people. The island is considered 20-th largest in the world and encompasses 84.421 squared kilometres.

- It is home to numerous castles,
- Irish people speak English but also Irish which is Gaelic language,
- St. Patrick is worldwide known Irish saint,
- Shamrock ☘ and leprechauns are integral and well known part of Irish tradition,
- Guinness beer best known Irish beer in world,
- It has oldest known pub 900 years old,
- Ireland has been inhabited approximately 7000 years,
are some of interesting facts about Ireland. [source](https://nationfacts.net/ireland-facts/)

Galway County, Ireland map.

![image.png](attachment:image.png)

### Problem
Apart from well known and worldwide recognized cultural, natural and historical treasuries of Ireland, that bring every year a numerous tourists from around the world, there is a question how much of these are still hidden, or properly represented and offered as tourist attractions. 
In this notebook I will try to give an answer to this question for Galway County.
I will go through Record of Protected Structurs in Galway County Ireland in order to see how much of them are still in use and their impact on local toursm. 

### Data acquisition and preparing

Data that will be used in this project are acquired from [Ireland's open data portal](https://data.gov.ie/). It holds more than 10000 dataset's divided between different sectors. 
    Data set used in this project contain information  about protected structures in Galway County provided by Galway Count Council. Information such as name and type of structure, address, geocordinates, date and identification number, current use, description, appraisal are ready to use.
    In order to extract and provide answer on actual treatment and inclusion in today tourist prospects of Galaway county they need to be slightly cleaned, and prepared for further use. 
    This means that some columns for this project was not be needed some have to be combined with different sources such as Foursquare app. 
    Complete dataset can be find [here](https://data.gov.ie/dataset/record-of-protected-structures1)

![image.png](attachment:image.png)

 After the first glimpse into the dataframe it was obvious that there where columns unnecessary for further examination. That is why they have been droped, and here is represented dataset whit necessary datapoints. There was 1514 rows and 20 columns. Building name, Appraisal, Curent Use, RMP number miss data, although for Current_Use column we can assume that respresents data about structures that are currently in use while rest is not.

According to this dataset there is a 108 different Building Types. Some of them with acctual number are shown below.

![image.png](attachment:image.png)

And those still in use are also represented:

![image.png](attachment:image.png)

Since OBJECTID uniformly designates every protected unit, regardless of missing data in other columns based on it can be determined number of currently used buildings enlisted in register of Protected structures.

![image.png](attachment:image.png)

Here is graphical representation of data from previous table.

![image.png](attachment:image.png)

## Methodology

The main idea behind this project is to compare data from two differente sources. One of them is dataset accured from Record of protected structures and the second one will be accured from Foursquare. 
Foursquare is worldwide recognized location platform that holds information about venues around the world. After visiting venues travelers leave information such as pictures, opinions, likes and dislikes or anything else they finde informativ for other users. 
The both sets should be cleand and prepared for further use aka comparison.
In the first step the dataset about Protected structures should be cleand and graphicly represented in order to make a clear picture about all registrated structures.
In the second step data for given geocordinates that represent Galway County will be pulled out from Foursquare website prepared for further use - represented as dataframe, and than based on common addresse or geocoordinates comparison will be made.

Map of Galway County with marked currently in use structures is shown below, followed by map oh Galway with marked all protected structures in this County 

![image.png](attachment:image.png)

![image.png](attachment:image.png)

From these two maps is clearly visible drastic difference between *All Protected Structures* and those amoung them currently in use. There is obviously a great potencial in representation of this richness through interesting stories and tours. Some of them also can have funcional use different from  that they have now, and their cultural, historical, or architectural value can be by this way utilized in more meaningful way.

As it was already said second step in this project is to pull data from Foursquare platform in order to make comparation with dataset acquired from Galway County Council. The results after comparation are as follows: 

![image.png](attachment:image.png)

For comparison in this case address was used as merging base. Only 5 of all registrated structures are found on Foursquare platform. Whether address or geocordinates have been used for merging datasets we came up with the same five location common for both datasets. With slightly different order of datasets before merging based on geocordinates we came up with this representation based on data from Foursquare platform.

![image.png](attachment:image.png)

## Results and Disscusion

After comparation has been made between two dataframes we finally have some numbers and they goes like this:

- 1514 Registrated protected structures according to dataset,
- 119 Registrated protected structures currently in use,
- 5 only amoung them are enlisted in Foursquare.

Only 7.86% from those recorded are currently in use. And only 0.33% from all recorded structures are worldwide visible throughout the Foursquare platform.

Although the number of currently used structures could be a higher than in dataset. The base for this assumption is grounded in results obtaind by merging two datasets based on geocordinates. Windfield House and L O'Brien House under the Current_Use column have NaN value for which I have made assumption that it means that these datapoints represent currently non used structures. Yet these Houses have appeared on Foursquare platform in category for Hotels.

Newertheless it's fairly small number if we take into the account complete list of Recorded structures, and as it could have been seen the list is quiet impressive. 

Reason for so small number of Protected Structures in some way included in tourism of Galway County can be numerus. And they ceartainly must be investigated in order to improve tourist offer of County.

Although results have shown that fairly small number of structures enlisted as protected by Galway County Council, that as such possess certain historical, cultural, architectural value, are presented as Tourist attracion. 

Lot's of at first sight, interesting buildings are not. Their inclusion in tourist offer of County can be benefitial from many aspects and one of main is Economic aspect for County, as well as budget for their preservation also educational character they can have for all that decide to see them. 
Those enlisted but not offered to a broader publicity represent potential that must be examined and included in Tourist prospects of County.
With broader offer cames more people who in that case usually love to stay a day or two more, who need to eat and if it's a local food than there is more job for local restorans as well as farmers. And this is not where chain is closed because  these people live traces - comments and pictures about places they have visited and draw another to follow them. 

Copyright zmajstorovic111@gmail.com, 2020.
