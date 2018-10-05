# SETUP

Download jar files in this checkout:

- [csvjdbc.jar](http://repository.hellonico.info/repository/hellonico/org/hellonico/csvjdbc/1.0.34_patched_01/csvjdbc-1.0.34_patched_01.jar)
- [metabase.jar](http://repository.hellonico.info/repository/hellonico/org/hellonico/metabase/metabase-01-83d1a40581400d46e58c6c528afc030496e408d0/metabase-metabase-01-83d1a40581400d46e58c6c528afc030496e408d0.jar)

# START METABASE

```
# start.bat 
# or
# start.sh
java -cp csvjdbc.jar:metabase.jar metabase.core
```

# BURGERS CSV DATABASE SETTINGS

Name:						burgers
Path to csv file:				BURGERS
fileExtension:				.csv
separator					,
quotechar					"
indexedFiles					YES
fileTailPattern				\.(.*)
fileTailParts					date
fileTailPrepend				NO
headerline
columnTypes					String,Double,Double,Double,Double,Double,Double,Double,Double,Double,Double,Date
suppressHeaders				NO
commentChar			
ignoreNonParseableLines		NO
missingValue				
trimValues					YES
Enable Logging				burgers.out
trimHeaders					YES
timestampFormat
timeFormat
dateFormat					yyyyMM

# sql query 


```
select * from BigMac where Country in ('Japan','France', 'Argentina');
```

# screenshot

![](burgers.png)