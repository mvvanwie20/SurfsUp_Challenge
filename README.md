# SurfsUp_Challenge
## Analysis
This analysis, requested by W. Avy, was meant to determine if a surf and ice cream shop would be sustainable year long in Oahu. In order to see if it was sustainable we were asked to determine the temperatures for the months of June and December. 

## Results
AS requested, I found the temperatures for the months of June and December and then produced a statistical analysis on the months temperatures. The results are as follows:

### June
- average temperature: 74.9 degrees F
- minimum temperature: 64 degrees F
- maximum temperature: 85 degrees F

### December
- average temperature: 71 degrees F
- minimum temperature: 56 degrees F
- maximum temperature: 83 degrees F

## Summary
According to the analysis I provided the surf and ice cream shop should be sustainable throughout the year based on temperature. It never drops below spring- like weather and the difference in max temperature throught the year seems to be about 2 degrees, meaning that it can be 80 degrees+ at any point in the year. If I were to add more queries I would also find the rain fall of June and December as well. While surferes may surf regardless of rain or shine, ice cream goers may be more deterred by the rain and so seeing if there is a distinct rainy season would help measure profitability. 

The two queries for rainfall would be as follows:

session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==6).all()


session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==12).all()
