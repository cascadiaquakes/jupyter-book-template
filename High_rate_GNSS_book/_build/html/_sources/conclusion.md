# Conclusion

All the notebooks are combined in a python script available here: https://github.com/UO-Geophysics/GNSS_ppp_high_rate/blob/main/process_ppp_linux.py  

The script needs the following arguments as input:  
* year: year to process
* nb_cores: number of core to run the PRIDE PPP in parallel
* testing: flag, if 0 it will process the full year, if 1 it will run on a subset of the year/stations
* restart: if the program stopped for any reason, the step where it stopped should be saved in the log file. setting restart to 1 will allow to restart where the program stopped and not from scratch

The script need the following files:  
* station_file = f'./station_lists/station_{year}.csv'  : csv with at least the column "station_id, readable with pandas
* token_path = "./" : path to the json with the token of your earthscope account

Outputs will be found here:  
* "./results_ENU": ENU position file
* "./results_XYZ": XYZ position file
    

## Publications

Here is the list of publications:


## Research team

CRESCENT