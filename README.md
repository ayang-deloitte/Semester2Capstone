# Home in the Outback: Predicting Housing Prices in Australia

Potential homeowners and renters in Australia face affordability concerns about housing combined with frequent underquoting of properties in the real estate industry, which makes determining the true price of a property paramount. Using sample Australian real estate data from Kaggle to predict prices based on factors such as listing agency, room number, and property type, buyers can more accurately determine which properties they can afford. Utilizing a gradient boosting model for regression, the model is able to account for 52% of price variability, and can provide a preliminary price guide for listings.

<img width="800" alt="Australian housing" src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/Elger_Street_housing_001.jpg/640px-Elger_Street_housing_001.jpg">

## Business Understanding

According to Statistia, housing affordability is a significant issue in Australia that has sparked many policy debates. Under 30% of Australians completely own their property, while approximately 30% of private households are composed of renters. As noted in the report, residental housing prices has typically seen strong annual growth, as have rental costs for the past decade [1]. This has led to several Australian cities such as Sydney and Auckland to be rated as some of the least affordable cities based on the ratio between housing prices and annual income [2].

<img width="512" alt="Least affordable housing in the world - Statista" src="https://cdn.statcdn.com/Infographic/images/normal/16902.jpeg">

Such an issue has also been compounded by the frequent practice of underquoting housing in the Australian real estate industry. Various organizations operating in the space have noted that "underquoting remains 'endemic' due to poorly regulated and underpoliced regulations". While the practice helps listers to gather more interested buyers, it also obfuscates the true price, creating much grief among hopeful buyers. As David Morrell, a buyers advocate in Australia, puts it: "It’s misleading, it’s a fraud on purchasers. And until significant penalties are handed out, regulations have been ineffective … if one does it, others have to follow" [3].

A housing price model can mitigate the issue until stronger laws punishing underquoting are passed. By estimating the price of housing through the usage of a model, buyers can more accurately determine which properties they can afford in the Australian real estate market. This saves them time searching through properties that have an unknown true price, while helping in spotting potential homes at a discount. 

## Data Understanding

The Kaggle [dataset](https://www.kaggle.com/datasets/thedevastator/australian-housing-data-1000-properties-sampled) used is a sample of 1000 Australian property listings. It contains information about the housing itself (such as size and amenities count) as well as housing type and product variation. This information can be used to specifically model prices for Australian housing based on common property aspects.

*insert EDA images*

Eight features were chosen for modeling housing prices. Building size, land size, and property type were chosen because housing size is a key component in determining property value. Bedroom, bathroom, and parking count can also affect housing value. Lastly, product depth may have an affect on how a property is marketed: housing considered "premiere" could have higher prices than those considered "standard".

One key limitation of the data is that the target variable (price) is based on property listings, which are subject to underquoting. It would be more accurate to model based on housing sold, but that data is not publicly availible for Australian housing. Because of that, the model will most likely predict pricing that is consistently less than the true value of the property. Additionally, the dataset is relatively small, and as such may be prone to overfitting. Managing this issue will require model regularization.

## Modeling & Evaluation

** rework baseline, maybe include linear regression later?
** neural net did not converge - so it is not included in this analysis
** in the real estate industry there are a few known aspects that affect price

## Conclusion

1) models do this better than the baseline, etc.

3) future work- can improve the model with the following


## Repository Navigation
### Info
### Links

#### Works Cited
[1] Granwal, L. *Residential housing market in Australia - statistics & facts*. Statista, 12 Dec 2022, [https://www.statista.com/topics/4987/residential-housing-market-in-australia/#topicHeader__wrapper](https://www.statista.com/topics/4987/residential-housing-market-in-australia/#topicHeader__wrapper). Accessed 2 Jan 2023.

[2] Buchholz, Katharina. *Where It’s Hardest to Afford a Home*. Statista, 21 Mar 2022, [https://www.statista.com/chart/16902/places-where-its-hardest-to-afford-a-home/](https://www.statista.com/chart/16902/places-where-its-hardest-to-afford-a-home/). Accessed 2 Jan 2023.

[3] Cassidy, Caitlin. *Underquoting in Australian real estate industry is leaving buyers feeling betrayed.* The Guardian, 26 Aug 2022. [https://www.theguardian.com/business/2022/aug/27/underquoting-in-australian-real-estate-industry-is-leaving-buyers-feeling-betrayed](https://www.theguardian.com/business/2022/aug/27/underquoting-in-australian-real-estate-industry-is-leaving-buyers-feeling-betrayed). Accessed 3 Jan 2023.

### Instructions

