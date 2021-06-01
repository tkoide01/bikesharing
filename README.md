# NYC Ciitibike Analysis

## Overview of the Analysis
Analyzing data from Citibike bike-sharing program in New York City area, provide the visualization of bike trip data to convince investors about launching a bike-sharing program in Des Moines. In order to do so, we will make following visualizations:  

1. Show the length of time that bikes are checked out for all riders and genders
2. Show the number of bike trips for all riders and genders for each hour of each day of the week
3. Show the number of bike trips for each type of user and gender for each day of the week.

Lastly, we combine these visualizations into Tableau dashboards and stories as final presentations for investors.
## Resources
- Data Source: 201908-citibike-tripdata.csv from the website *Citi Bike System Data* URL: <https://www.citibikenyc.com/system-data>
- Software: Jupytor Notebook, Tableau Public

## Results:
Followings are the seven visualizations for the NYC Citibike analysis and desctiption for each visualization:

1. **Gender Breakdown**
- As shown on the visualizaion, we see that majority of Citibike users were male. Be more specific with number, the breakdown is male: 1,530,272, felamle: 588,431, and unknown: 225,521. In percentae, male: 65.27%, female: 25.10%, and unknown: 9.62%.

![](images/gender_breakdown.png)

2. **Checkout Times by Gender**
- The line diagram is displaying three different lines by gender. Although, the line for male is significantly bigger in terms of 'Number of Bikes,' the shape of lines are almost identical between male and female, which means both male and female tend to have similar characterstics in checkout times. Therefore, we do not see much reason to prefer certain gender over the other for checkout time.

![](images/checkout_by_gender.png)

3. **User Type**
- The pie chart shows that over 81% of customers are subscriber to the program and only 19% of the customers are non-subscriber. This result suggests that the business model should encourage users to sign up subscription and also provide service to maintain them to be successful.

![](images/customer_breakdown.png)

4. **Top Starting Locations**
- The map plots starting station locations in NYC. Note that plotted points are differenciated by color and size based on their used counts. We can see that large dots are plotted mainly 50th street and below in Manhattan.

![](images/top_starting_locations.png)

5. **Trips by Weekday for Each Hour**
- The heatmap displays how bike usage is populated by weekday for each hour. We can see that there are two peaks in weekdays around 7AM-9AM and 5PM-7PM while the peaktime is spread throughout the day for weekend. This means that users are often using for commute in weekdays and thus there are two peaks during those time frames.

![](images/trips_by_weekday.png)

6. **Trips by Gender (Weekday per Hour)**
- The heatmaps are adjusted from the previous visualization that the maps are separated by gender. Similar to what we saw for the **Checkout Times by Gender**, the gradation in heatmaps we see is almost identical among all genders. Thus, both male and femal rides bike in the same timeframes.

![](images/trips_by_weekday_gender.png)

7. **User Trips by Gender by Weekday**
- The heatmap displays user trips separated by gender and by type of subscription. One thing we notice is that we have lot less 'unknown' subscriber compared to non-subscriber customers. This do make sense since people more likely to register their gender when they sign up as subscriber.

![](images/user_trips_gender.png)



## Summary
Based on the visualizations produced on Tableau based on NYC Citibike usage data, we summarized in two dashboards as below
1. **Gender Analysis**
[link to dashboard](https://public.tableau.com/app/profile/takuma.koide/viz/bikesharing_challenge_16225734714640/GenderAnalysis "Gender Analysis")
- The dashboard display show three images that analyze the bike users by gender. In summary, the number of male users exceeds more than double of the female user number. On the other hand male and female users are very similar in checkout time (most users ride for 5-6min) and when to ride a bike (both genders ride bike for commute reason during weekday and their peaktime spreads out in weekend).
- Given the above analysis, we should strategize the marketing of the bike-sharing program in Des Moines mainly to male users as this demographic is more likely to use bike for tranportation than femal.
- Also, bike stations should be located to spots where faciliate people's commute. So if people tend to come work to Des Moines by train and then walk from there to their job, then we should build bike stations near by those train station.
- For the future analysis, we should make research on potential of bike-sharing program to female customers and identify key reason of imbalance usage of bike-sharing between male and female. If both user categories ride bikes in a similiar way, why one group choose to ride bike more often? Could it be how NYC Citibike was promoted? Or is it due to how female does dress or make-up which could be difficult to control? Depends on the potential in female users, we could expand the bike-sharing program business.

2. **Subscriber Analysis**
[link to dashboard](https://public.tableau.com/app/profile/takuma.koide/viz/bikesharing_challenge_16225734714640/SubscriberAnalysis "Subscriber Analysis")
- The analysis shows that nire than three quarters of users are subscribed user. Also, among the gender segmentation, male user is more likely subscriber compared to female and unknown users.
- Given the observation, the key factor to be successful in bike-sharing program is how much subscriber you can have in the area as they utilze bike-sharing much more often compared to non-subscriber. Therefore, we need to consider two things: how to turn users to subscriber and how to maintain them as a subscriber.
- From the map of the 'Top Starting Locaitons' we can find that popular locations are inside Manhattan in NYC. Also, 'User Trips by Gender by Weekday' presents that subsribed users are often riding bike in weekday compared to weekend. Therefore, we can assume that there is an overlap between commuter population and subscibers. Thus we should utilize advertisements inside city, train stations, trains to approach commuters. In addition, we should integrate reward system or discount for long-term subsribers to maintain their subscription.

