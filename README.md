# Surfs-Up-Challenge
## Overview of the analysis: Explain the purpose of this analysis.
The Purpose of the analysis is W. Any wants more information about temperature trends before opening up the surf shop. He wants temperature data from June and December in Oahu, so he can determine if he should keep the surf and ice cream shop business open all year round. 
## Results: Provide a bulleted list with three major points from the two analysis deliverables. Use images as support where needed.
1. As the images show below the mean temperature in June is 74.9 and the mean temperature in December is 71.04, which is not drastically different. 

<img width="172" alt="Screen Shot 2023-01-03 at 10 55 07 AM" src="https://user-images.githubusercontent.com/110268006/210393620-b27275fa-ffed-4aa0-ae6e-55c81506ba24.png">
<img width="175" alt="Screen Shot 2023-01-03 at 10 55 16 AM" src="https://user-images.githubusercontent.com/110268006/210393698-b848e256-e341-4eac-b096-1eb5787c0d51.png">

2. Looking at the minimum temperatures as the image below shows in June it is 64 and in December it is 56, which is a 9 degree difference. This could deter some people from surfing and eating ice cream. 

<img width="177" alt="Screen Shot 2023-01-03 at 10 55 25 AM" src="https://user-images.githubusercontent.com/110268006/210394022-9b538e7c-9440-488b-9949-f2971cb48c09.png">
<img width="191" alt="Screen Shot 2023-01-03 at 10 56 26 AM" src="https://user-images.githubusercontent.com/110268006/210394087-66538d3d-6c25-497e-a609-f394d0a832c1.png">

3. Looking at the maximum temps for both months shows there is not a big difference, in June the max is 85 and in Dec the max is 83.

<img width="173" alt="Screen Shot 2023-01-03 at 10 55 55 AM" src="https://user-images.githubusercontent.com/110268006/210394265-83e7a84b-ec81-45e1-857e-590f549f4c33.png">
<img width="209" alt="Screen Shot 2023-01-03 at 10 56 29 AM" src="https://user-images.githubusercontent.com/110268006/210394274-6cb8c711-db02-492c-8dc2-42b437f062aa.png">

## Summary: Provide a high-level summary of the results and two additional queries that you would perform to gather more weather data for June and December.
I don't think the temperature would have much of an impact itself because there wasn't a huge difference in temperature from June to December, execept for the minimum temerpature which was a 9 degree difference and that could deter invidiuals from surfing and eating ice cream. It may have a little impact but another area of concern would be preceiptation and so I added queries on precipitation because people may be less likely to surf and eat ice cream in the rain. 
### 1st query
results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==6).all()
results
### 2nd query
results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==12).all()
results
