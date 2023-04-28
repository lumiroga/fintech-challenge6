# Challenge VI | PyViz Visualization Tools |Fintech <img src="https://instructure-uploads-pdx.s3.us-west-2.amazonaws.com/account_150420000000000001/attachments/590996/columbia.png" height="48" width="48">

---

This is the 6th challenge, now for evaluating the housing market in San Fracisco
For the analysis a better set of plotting tools, including geographic mapping tools, is used to have a better idea of the data and its patters across the time.

The data sources are the following

- **San Francisco Neighborhoods list and coordinates**            
- **Sales Price per square foot and Rent every year from 2010-2016 for every neighborhood**    
- **Crypto Currencies (ETH & BTC)**    

---

## Libraries Used

The main language is Python embeded in Jupyter lab

### jupyter

This modules creates a notebook and processes a python kernel.

### pandas

Library that handles Dataframes and Series to process data, filter, create statistics

### hvplot

Library to plot graphs, enhanced graphics and options

### pathlib

Library for path logic and OS differences abstraction


---

## Usage

To run program just open the terminal (anaconda needs to be installed) and type the following

``` bash
$ git clone https://github.com/lumiroga/fintech-Challenge6.git
$ cd fintech-Challenge5
$ jupyter lab 

```

Open a browser with the displayed URL in Jupyter

Look for *san_francisco_housing.ipnyb* file and open it.

---
# Graph Units per Year

The graph shows the amount of units in the city for each year

# Graph Price per Square foot vs Monthly Rent

The graph shows the price per square foot and rent for each year.

## Graph Price per Square foot grouped by Neighborhoods.

The graph shows the price per square foot and rent for each year with a widget to filter each specific neighborhood and compare the different trends between neighborhoods in an interactive way.

# Graph Price per square foot and montly rent in a map with neighborhood locations.

The graph shows the price per square foot and rent for each year with an interactive map where neighborhoods are mapped with coordinates and the size represents the price per square foot.

## Contributors

[lumiroga](https://github.com/lumiroga)
[Stack overflow](https://stackoverflow.com/questions/59678780/show-extra-columns-when-hovering-in-a-scatter-plot-with-hvplot)

---

## License

* mpl-2.0 | Mozilla Public License 2.0