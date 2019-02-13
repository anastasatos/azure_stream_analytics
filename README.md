# Azure Stream Analytics

## SCENARIO:

*Azure Stream Analytics to process a data stream of vehicle observations and answer stream queries.*

You have access to a data stream that’s generated from sensors placed in some checkpoints (toll stations and speed cameras). Each time a car passes by one checkpoint, an event is generated. All cars are equipped with tags that provide the vehicleTypeID and colorID of each car. Tag readers are capable of reading this information. In addition, a camera reads the license plate and completed the event’s data. You are asked to create an Azure Analytics solution for the tasks listed below:

- Query 1: In a tumbling window of 1 minute count the number of Audis that passed through a toll station. 
- Query 2: In a hopping window of 3 minutes, for each color, calculate the total number of cars that passed through a police speed limit camera. Repeat every 90 seconds. 
- Query 3: In a tumbling window of 20 seconds, for each color, find the oldest car that passed through a toll station. 
- Query 4: In a sliding window of 60 seconds, calculate the speed limit camera spots where the most violations happened. 
- Query 5: In a sliding window of five minutes, for each color and car model, display the total number of cars that break the speed limit. - Query 6: You have been given a list of the license plates of police’s most wanted criminals. In a sliding window of 1 minute, display a list of all the cars that you spotted at any checkpoint. 
- Query 7: In a sliding window of 1 minute, display a list of fake license plates. Check if the same license plate has passed through any type of checkpoint twice in the same time window. 
- Query 8: In a tumbling window of 2 minutes, calculate the percentage of BMW drivers that break the speed limit. (eg Out of all the BMW drivers that were identified in the last 2 minutes, 80% broke the speed limit).
