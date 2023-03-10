# Network
# Availability
This program calculates yearly and monthly availability of a certain network, with output tables and charts. 

Availability is how a network (roads, trains, trams...) is negatively influenced with segments having a low speed and/or total blocks (e.g. due to construction sites; these impede the regualar effort of the network.)

## Purpose of the project
If your network never works at maximum efficiency all the time;
If you are a construction service industrial company;
If your clients want to know when you are going with the new innovations;

This is a project you might be curious with;
Total or partial blocks having negative influence the efficiency of the network will underperform your network's availability; 
you will hear users complaining as well!

If thy goal is maximising the efficiency of the network;
If thou want to know: "is my network available?"
"Are there seasonality patterns that emerge? Do certain months perform better than others?"
"How much will our construction works with next year's planning impact the network efficiency (and customer satisfaction)? "


Your boss will be curious of having a read of this program comes into play...

### A simple solution to calculate the network availabiltiy
Wether you are the Swiss [SBB CFF FFS](https://company.sbb.ch/en/home.html), the French [SNCF](https://www.sncf.com/en) or the Italian [Trenitalia](https://www.trenitalia.com/en.html), you are interested in knowing how your network is performing.

You can now use this algorithm to automatically crunch the numbers of your data and come up with a simple and replicable solution to draw conclutions from your data.

Just provide a shapefile of the network and shapefiles of the tracks that limit the availability of the network (be them slow-speed segments and total-blocks.)

Run the algorithm in a [Jupyter Notebook](https://jupyter.org/) or on [GoogleColab](https://colab.research.google.com/).

Enjoy automatically created tables with availability data and charts that graphically tell the story about them.

Use these data to make informed and better decisions.

To the success of your network!

But how does the whole thing work? Read on...


## Technology
### Interpreter
Python 3.9.7

### Python libraries
Install the following libraries before running the script:
* [pandas](https://pandas.pydata.org/)
  * Install anaconda or miniconda as described [here](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html), then open a terminal and run:
  ```
  $ conda install pandas
  ```
* [openpyxl](https://openpyxl.readthedocs.io/en/stable/)
  * In a terminal, run:
  ```
  $ pip install openpyxl
  ```
* [ua_parser](https://github.com/ua-parser/uap-python)
  * In a terminal, run:
  ```
  $ pip install ua_parser
  ```
* [matplotlib.pyplot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.html)
  * In a terminal, run:
  ```
  $ python -m pip install -U pip
  $ python -m pip install -U matplotlib 
  ```

## Usage example
1. Create a folder with [ua_parsing.py](https://github.com/lucalevi/User-agent-parser/blob/main/ua_parsing.py) and your Excel table of UserAgents and relative count number (cnt). We will use [Unique_UserAgents_sample.xlsx](https://github.com/lucalevi/user-agent-parser/blob/main/sample_data/Unique_UserAgents_sample.xlsx).
2. In the [script](https://github.com/lucalevi/User-agent-parser/blob/main/ua_parsing.py), you can adapt the following lines according to your need, if you want different output file names 
```python
outputFileName = 'Unique_UserAgents_parsed.xlsx'
osFile = 'OS_count.xlsx'
browserFile = 'browse_count.xlsx'
deviceFile = 'device_count.xlsx'
plotOsFileName = 'piechart_os.png'
plotBrowserFileName = 'piechart_browser.png'
plotDeviceFileName = 'piechart_device.png'
```
3. Open a terminal in the created folder and run:
```
python3 ua_parsing.py yourfilename.xlsx
```
4. If you use the data of this example, you can sobstiute yourfilename.xlsx with Unique_UserAgents_sample.xlsx (which is [this](https://github.com/lucalevi/user-agent-parser/blob/main/sample_data/Unique_UserAgents_sample.xlsx) file)
5. As output, you will have an Excel table of the parsed UserAgent data ([here](https://github.com/lucalevi/user-agent-parser/blob/main/results/Unique_UserAgents_parsed.xlsx) an example).
![Parsed UserAgent data](https://github.com/lucalevi/user-agent-parser/blob/main/sample_img/Unique_UserAgents_parsed.png "Parsed UserAgent data")

6. Afterwards, some statistics are calculated to verify the shares in the data among the Operative Systems, browsers and device type used. 
 * The script outputs three Excel tables, one for each share (OS, browser, device type)
  
 ![Example of output table](https://github.com/lucalevi/user-agent-parser/blob/main/sample_img/OS_count.png "Example of OS output table")
 * it plots the data graphically with pie charts.
 ![Example of OS share pie chart](https://github.com/lucalevi/user-agent-parser/blob/main/results/shares_img/piechart_os.png "Example of OS share pie chart")


## What's in this repo
The main files in this repo are:
* [ua_parsing.py](https://github.com/lucalevi/User-agent-parser/blob/main/ua_parsing.py): the Python script that parses the user agent data.
* [Unique_UserAgents_sample.xlsx](https://github.com/lucalevi/user-agent-parser/blob/main/sample_data/Unique_UserAgents_sample.xlsx): sample table of unique UserAgents and their relative count number (these are e.g. counts of how many unique UserAgents clicked on a certain web page.)
* [Unique_UserAgents_parsed.xlsx](https://github.com/lucalevi/user-agent-parser/blob/main/results/Unique_UserAgents_parsed.xlsx): output table of the parsed data. It contains multiple columns with information about Operative System, browser and device type used, together with the count number of the input table.
* [OS_count.xlsx](https://github.com/lucalevi/user-agent-parser/blob/main/results/shares_tables/OS_count.xlsx), [browse_count.xlsx](https://github.com/lucalevi/user-agent-parser/blob/main/results/shares_tables/browse_count.xlsx) and [device_count.xlsx](https://github.com/lucalevi/user-agent-parser/blob/main/results/shares_tables/device_count.xlsx): three sample output tables calculated by the script. They are obtained by a groupby() function.
* [piechart_os.png](https://github.com/lucalevi/user-agent-parser/blob/main/results/shares_img/piechart_os.png), [piechart_browser.png](https://github.com/lucalevi/user-agent-parser/blob/main/results/shares_img/piechart_browser.png) and [piechart_device.png](https://github.com/lucalevi/user-agent-parser/blob/main/results/shares_img/piechart_device.png): the pie charts plotted based on the output tables of the previous point.


### Which OSs, browsers and device types are included in the data analysis?

#### OSs: 
* Windows
* iOS
* Mac
* OS X
* Android
* Linux

#### Browsers: 
* Firefox
* Chrome
* Safari
* Opera
* Edge

#### Device types:
* Computer
* Mobile (smartphones + tablets)



## Meta

Author: Luca Iacolettig - iacolettig(dot)luca(at)gmail.com

Distributed under the GNU GPL v3 license. See [LICENSE](..User-agent-parser/LICENSE) for more information.
