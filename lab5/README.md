## Task 1 
Is done in 7.5
I created the "delivery_speed_km_per_min" feature to capture the operational efficiency of each trip. While distance and duration are useful independently, their ratio provides a clearer picture of the delivery conditions. A very low speed might indicate heavy traffic congestion. 
---------------------------------------------------------------------------------------------------------------------------------------------------------
## Task 2 
Is done in 7.0
"is_peak_hour" is modified from 12-15 (lunch) and 19-23 (dinner). "To 17:00 (5 PM) to 22:00 (10 PM)". Performance is not changed from 5-10 PM
---------------------------------------------------------------------------------------------------------------------------------------------------------
## Task 3
Is done in 7.4
Where Changing the "top_k" value didn't impact performance because the dataset only contains 9 unique items. Since the chosen thresholds were higher than the total number of categories, all items were preserved and none were grouped into "Other,".
---------------------------------------------------------------------------------------------------------------------------------------------------------
## Task 4
Is done in 7.3
The optional feature selection was "not beneficial" because the model's accuracy remained identical. The "haversine_rest_to_cust_km" feature proved redundant; when removed, its importance score (0.062) was simply "absorbed by Delivery_Distance_km", which rose to 0.071. Since the model just reallocated the same predictive weight to a similar distance metric, the final performance stayed the same.
