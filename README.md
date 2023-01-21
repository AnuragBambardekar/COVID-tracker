# COVID Tracker using SpringBOOT
- Initialized the project using STS4 [Spring Tool Suite 4], which is a Eclipse extension for initializing SpringBOOT projects <br>
- Can alternatively use Spring Initializer tool. <br>
- Project was done during the pandemic. <br>
- This application lists the current number of cases reported across the world <br>
- Data from Johns Hopkins University COVID-19 cases which is hosted on their GitHub repository <br>

### Project Screenshot:
![Project](/coronavirus-tracker/Images/app_op.png?raw=true "COVID-19 Tracker deployed on localhost")

### Running the project:
- Project uses JAVA 11
- Maven build
- Maven Install
- Go to main file
- RC and Run as Java Application

### Learning Outcomes:
- Spring BOOT Annotations <br>
- Model - View - Controller architecture <br>
- Maven <br>
- Fetching Data using HTTP calls (@PostConstruct) <br>
- Parsing the data using CSV <br>
- BootStrap for simple frontend design <br>
- Automatic Updation using @Schedule annotation by using cron expression <br>
- cron expression is a string which specifies the time, which can be then used to schedule the method to run (which fetches COVID-19 data) after a specified amount of time. <br>
- @Scheduled(cron = "* * * 1 * *")  [minute, hour, day-of-month, month, day-of-week, command] <br>

**What is inside?**
- model file has the getter-setter methods for country, state, total cases, and the difference in cases from previous day and current day. <br>
- controller file has the lists for the data and calling the methods to get the data. <br>
- service file has the business logic which has the HTTP calls to fetch the data and parsing the data. <br>

**Future Scope:**
- Create some visualizations to get a better understanding of data for better interpretability, because inferring information from large data can be time consuming. <br>
- Deployment

#### Resources:
- https://www.youtube.com/watch?v=8hjNG9GZGnQ&t=850s - Tutorial for this Project by Java Brains

- https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_global.csv

- https://github.com/CSSEGISandData/COVID-19 - Novel Coronavirus (COVID-19) cases, provided by Johns Hopkins University CSSE