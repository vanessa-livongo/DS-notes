# Dashboard Design Process
- [Link](https://dataschool.com/how-to-design-a-dashboard/dashboard-design-process/)

## Process
1. Define
2. Prototype
3. Build
4. Deploy

<img src="https://dataschool.com/assets/images/how-to-design-a-dashboard/dashboard-design-process/dash-design-process-overview.jpg" height="300px">

## 1. Define
_Who this dashboard is for and what metrics matter to them_

### Stakeholders
- The designer (you)
- The audience
- The point person (the member of audience who has the most experience)
- The Data Gatekeeper (the member of the data team who will help withh the database)

### Define the Decisions
- Worst Case Scenario: how did this happen? What decisions led to this outcome? Waht decisions were made with a lack of data?
- Prioritize decisions

### Define the Metrics
- What data would help inform that decision?
- What other data might be useful to add context?
- How else could we improve this decision’s quality?
- <img src="https://dataschool.com/assets/images/Screen%20Shot%202020-02-10%20at%201.58.58%20PM.png" height="200px">

## 2. Prototype
### Selecting Visualizations
<img src="https://dataschool.com/assets/images/Decision%20Tree%206.png" height="500px">
- Consider limiting the number of categories by using an “Other” bucket, color the Other column grey to deemphasize this category, since it is a grouping of multiple categories

### Alignment & Grouping
- If a specific metric is displayed in two charts, they should be placed right next to each other
- Line charts with the same time frame should be stacked vertically to facilitate comparisons
- Put items next to each other with no separation to use the same title for both visualizations
  <img src="https://dataschool.com/assets/images/how-to-design-a-dashboard/arranging_your_charts_as_a_dashboard/sameTitle.png">

### Limited Variety
- The average viewership peaks when six different types of charts are used

### Review
- Gather documents stating the goal, decisions, and metrics

## 3. Build
### Find the Data
- Do we have the data available
- Where is the data stored
- Is the data messy

### Messy data
- Missing values: ignore, delete, impute
- Wrong values
  - Fake phone number
  - Fake names
  - Fake birthday: too young, too old
- Potentially Wrong values
  - Outliers: IQR = Q3 - Q1, [Q1 - 1.5 * IQR, Q3 + 1.5 * IQR]
  - Various capitalization
  - Misspellings
  
### No data
- Track new data points
- Proxy metrics: that give similar information
  
## 4. Deploy
- Context
- Medium
- Scheduling

### Context
- Descriptive chart titles
- Label axes
- Provide a legend
- Add Definitions: Adding a short description beneath the metric clarifies the information that is represented and its limitations

###  Medium
- Email
  - Can this dashboard be shared externally?
  - What level of access do people need to view the dashboard?
  - How frequently should I send out the data so that people don’t ignore it? (align the schedule with the frequency of decisions being made from the dashboard)
  
### Scheduling
- Scheduling should mimic the pace at which decisions need to be made
- If people do not need to view the dashboard to make a decision unless a metric changes dramatically, set up an alert

###  Scaling
- Adding links, interactivity, and documentation
- Optimizing queries
  - go to the Data Gatekeeper to discuss creating a pre-aggregated table that you can query from
- Removing unused dashboards
- Documentation

### Maintenance
- Setting up scheduled times to review
  - Total dashboard views
  - Repeat dashboard views
  - Unique dashboard viewers
  - Do queries produce expected results?
  - Have the underlying data sources or data models for this dashboard changed?
- Providing a way for audience to provide feedback
