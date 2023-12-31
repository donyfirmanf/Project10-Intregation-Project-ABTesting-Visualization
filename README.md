# Project10-Intregation-Project-ABTesting-Visualization

### Description of the data

Each log entry is a user action or an event. 

- `EventName` — event name
- `DeviceIDHash` **— unique user identifier
- `EventTimestamp` — event time
- `ExpId` — experiment number: 246 and 247 are the control groups, 248 is the test group

### Instructions for completing the project

**Step 1. Open the data file and read the general information**

File path: *`/datasets/logs_exp_us.csv`*

**Step 2. Prepare the data for analysis**

- Rename the columns in a way that's convenient for you
- Check for missing values and data types. Correct the data if needed
- Add a date and time column and a separate column for dates

**Step 3. Study and check the data**

- How many events are in the logs?
- How many users are in the logs?
- What's the average number of events per user?
- What period of time does the data cover? Find the maximum and the minimum date. Plot a histogram by date and time. Can you be sure that you have equally complete data for the entire period? Older events could end up in some users' logs for technical reasons, and this could skew the overall picture. Find the moment at which the data starts to be complete and ignore the earlier section. What period does the data actually represent?
- Did you lose many events and users when excluding the older data?
- Make sure you have users from all three experimental groups.

**Step 4. Study the event funnel**

- See what events are in the logs and their frequency of occurrence. Sort them by frequency.
- Find the number of users who performed each of these actions. Sort the events by the number of users. Calculate the proportion of users who performed the action at least once.
- In what order do you think the actions took place. Are all of them part of a single sequence? You don't need to take them into account when calculating the funnel.
- Use the event funnel to find the share of users that proceed from each stage to the next. (For instance, for the sequence of events A → B → C, calculate the ratio of users at stage B to the number of users at stage A and the ratio of users at stage C to the number at stage B.)
- At what stage do you lose the most users?
- What share of users make the entire journey from their first event to payment?
