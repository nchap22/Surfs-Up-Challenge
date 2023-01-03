# Surfs-Up-Challenge
## Overview of the analysis: Explain the purpose of this analysis.
The Purpose of the analysis is W. Any wants more information about temperature trends before opening up the surf shop. He wants temperature data from June and December in Oahu, so he can determine if he should keep the surf and ice cream shop business open all year round. 
## Results: Provide a bulleted list with three major points from the two analysis deliverables. Use images as support where needed.
1. As the images show below the mean temperature in June is 74.9 and the mean temperature in December is 71.04, which is not drastically different. 
2. Looking at the minimum temperatures as the image below shows in June it is 64 and in December it is 56, which is a 9 degree difference.
3. Looking at the maximum temps for both months shows there is not a big difference, in June the max is 85 and in Dec the max is 83
4. Summary: Provide a high-level summary of the results and two additional queries that you would perform to gather more weather data for June and December.
Maybe looking at precipitation because people may be less likely to surf and eat ice cream in the rain. 
### 1st query
results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==6).all()
results
### 2nd query
results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==12).all()
results
