# Analysis on schools in a district
## Overview of the school district analysis
I have the data retrieved from math and reading scores from 15 schools and from four different grades. I want to make an analysis based on this data to see the best performing schools by diferent categories based of the scores of the students. Another problem that came up was that the scores for the 9th graders at Thomas High School may have been altered and it is necessary to ignore this data for our analysis.
## Results
- How is the district summary affected?

  To see how much the altered grades affect the district summary, let's take a look to the following images:
  
  ![image](https://user-images.githubusercontent.com/89402038/136705933-884f2b68-1d82-407f-9159-1d653e6434fe.png)
  
  ![image](https://user-images.githubusercontent.com/89402038/136705854-dcc7e837-f331-43a1-908f-a794a095e315.png)
  
  In the first image is shown the district summary taking into consideration the scores from Thomas High School's 9th graders and in the second image this scores were asign a value of Na and not taken into consideration for the summary. As we may see there is a bit of a dip overall except for the _Average Reading Score_ but this overall dip in the other categories is just a few tenths that could mean not so much importance taking into consideration the amount of data collected. 
- How is the school summary affected?
  
  In the same way as to the district summary let's take a look to the before and after the scores were modified:
  
  ![image](https://user-images.githubusercontent.com/89402038/136706436-03435e08-00e9-4bfa-b70a-9d7def65033e.png)
  
  ![image](https://user-images.githubusercontent.com/89402038/136706518-e640b172-f19d-448a-bd31-de6324c2061a.png)
  
  We are taking only a look to the Thomas High School's data because the other schools suffered no change at all.
  This adjustment hits pretty hard the _% Passing Math_, _% Passing Reading_ and _% Overall Passing_ bringing them from overall 90s to 60s. The averages do not suffer any big change. To make up for this erroneous data I adjusted the analysis to not take into consideration the 9th graders' and obtained the following new data:
  
  ![image](https://user-images.githubusercontent.com/89402038/136706778-af115634-cd90-4701-aea2-b9f38c3e89de.png)
  
  As we may see the previous categories that were hugely affected by the changed returned to values similar to their previous ones, just different by a few tenths.
- How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?
  
  For this analysis lets see first the full picture:
  
  ![image](https://user-images.githubusercontent.com/89402038/136706991-2970e240-eb84-4153-b42f-6caf726ceabc.png)
  
  The table shows the schools ordered by _% Overall Passing_ in a descending order with the latest changes made to the Thomas High School in order to make up to the altered data. We may see that here the school is placed in a tight second place above the third school by just a tenth. If the 9th graders' scores would be taken into account, the Thomas High School would have a little bit bigger lead in second place by four tenths. Therefore the actual table represents an accurate representation of where the Thomas High School is respectively to the other schools in the district.
- How does replacing the ninth-grade scores affect the following:
  - Math and reading scores by grade
    
    ![image](https://user-images.githubusercontent.com/89402038/136707720-2b86a542-071f-4a9e-9c81-627207938301.png) ![image](https://user-images.githubusercontent.com/89402038/136707734-059a9920-9b52-49bd-b247-f2550622bf87.png)
    
    Here it is shown on the left image the math score average for each school and grade and on the right image are the reading score averages. Here the only minor change is in the both Thomas High School 9th graders average score is substituted with a "nan", which implies a not a number value. 
  - Scores by school spending
    
    For this part four ranges were created to categorize each school. The ranges are: <$584, $585-629, $630-644 and $645-675. The values of this ranges were determined by the statistical analysis on the _Per Student Budget_ values. The lowest value is 578, the highest value is 655 and the standard deviation is 28.5 aproximadetly 30. Then establishing the lowest limit as 578 would only mean having one school inside that range therefore 584 is established as the lower limit because then we would have four schools inside that range. Afterwards, because the standard deviation is 30, I increased the bins by 30 up to 675.
    
    ![image](https://user-images.githubusercontent.com/89402038/136709331-3e394cb5-9107-445b-aded-fc6c0cd5aca0.png)
    
    The table shows all the schools  and their respective values and it is ordered in descending order based on the _% Overall Passing_ values. Here we can see the that the top school is one  of the schools that spend less per student. A clear sign that spending more does not imply better performance. None of the top schools are in the higher ranges of spending. The previous point can be seen in the following table:
    
    ![image](https://user-images.githubusercontent.com/89402038/136711741-e061f057-0a24-413e-b573-11028ce5a7fa.png)
    
  - Scores by school size
    
    Following the same procedure as the previous point, the ranges were established as follows: Small (<1000), Medium (1000-2000) and Large (2000-5000). And the results were the following.
    
    ![image](https://user-images.githubusercontent.com/89402038/136712021-a14d0e88-7abb-4c19-ae5c-1600b6384c70.png)
    
    As we may see from the previous table the schools with the better performance were the medium ones, but the small ones are not to far behind. But what is surprising is the low overall passing percentage of the large schools. This shows that the bigger schools are having trouble focusing efficiently their resources to improve this stat.
  - Scores by school type
    
    The ranges for the following analysis are just by "Charter" and "District" and the table is:
    
    ![image](https://user-images.githubusercontent.com/89402038/136712193-8152e495-f498-4c52-bea8-823c802526c9.png)
    
    From the table we can see that the overall passing percentage for the "District" type is very low. Focus must be placed on improving the math average and the passing percentage for math.
## Summary
In conclusion big budgets does not always mean big improvement, the data analysed is just a snapshot of what is happening. A suggestion could be to keep a watch on trends for the schools with bigger budgets to see if they improve or not. If not a suggestion would be to minimize the budget therfore pushing to a more efficient use of the resources. Also bigger schools tend to have bigger problems than smaller or medium ones, especially in maths. The focus of this schools should be in improving their math scores and keep doing the same work in reading in the short term. In the long term this schools should look forward to improve both reading and maths because they are still lagging behind in comparison to the other schools.
