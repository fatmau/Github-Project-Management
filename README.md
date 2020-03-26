# Github-Project-Management
a set of notebooks to gather data from Github &amp; Zenhub and plotting cycle time


## zenhub_github_data_import
this notebook gets all issues and their cycle times, event dates from Github & Zenhub. As an outcome, it creates a csv file contaning most details of any story in your github directory.

WARNING: Do not forget to edit your project parameters in the first cell


## cycle_time_scatter_diagram
In this notebook, main goal is generating a project diagram displaying daily mean/Q1/Q3/std of story cycle times by;

* reading issue data from a csv file
* calculating daily mean/Q1/Q3/std
* calculation all time averages of cycle time
* plotting all findings on a single diagram

NOTE: this notebook needs a csv file like the one exported by zenhub_github_data_import, please first run that notebook first.


## monte_carlo_simulations
2 different types of Monte Carlo simulations are executed and diagrams are plotted.

NOTE: this notebook needs a csv file like the one exported by zenhub_github_data_import, please first run that notebook first.

### Monte Carlo Simulation for certain amount of items
Based on the throughput data we simulate multiple times how many items can be completed in the given time span. Before we run the simulation we set the configuration values:

* Date range of data basis
* Number of days to simulate (probably an iteration or release window)
* Number of simulations to run (Recommendation: >= 10000).

### Monte Carlo Simulation for time window
Based on the throughput data we simulate multiple times when the number of items will be completed. Before we run the simulation we set the configuration values:

* Date range of data basis
* Number of items to simulate
* Start date of work
* Number of simulations to run (Recommendation: >= 10000).

