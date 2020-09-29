# Zabbixhistory2csv

This tool is used to pull history from the zabbixapi by itemid and output to csv file.  
  
Tested on python2.7 with zabbix2.2.  

## Usage:
```
usage: zabbixhistory2csv.py [-h] [-V {True,False}] -H HOST [-u USER]
                            [-m MINUTES_AGO] [-o OUTPUT_FILE] -i ITEMID

zabbixhistory2csv

optional arguments:
  -h, --help            show this help message and exit
  -V {True,False}, --verify {True,False}
                        Verify SSL (True, False) (default: True)
  -H HOST, --host HOST  Zabbix API hostexample:
                        https://zabbixhost.example.com/zabbix (default: None)
  -u USER, --user USER  Zabbix API user (default: anthony)
  -m MINUTES_AGO, --minutes-ago MINUTES_AGO
                        How many minutes worth of history shouldbe returned
                        going back in time from right now (default: 60)
  -o OUTPUT_FILE, --output-file OUTPUT_FILE
                        Output file in csv format Default: output.csv
                        (default: output.csv)
  -i ITEMID, --itemid ITEMID
                        The zabbix item that we will use in our history.get
                        api call. (default: None)
```

## Installation of dependencies:
pip install -r requirements.txt

## Input time needs to be offset by timezone!!
