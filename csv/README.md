# use logstash to import csv to elasticsearch

### file input
file input runs logstash as long running process, so if you just need it once, use stdin input    
logstash -f csv\csv2es-file.conf    

### stdin input    
stdin input allows us to use import as one-short and shutdown automatically 
###### on windows, [how to pipe file to command](http://www.lagmonster.org/docs/DOS7/pipes.html#pipe)    
    logstash -f csv\csv2es-stdin.conf < I:\dev\softpack\noosh_elasticsearch\logstash-2.0.0_csv\bin\csv1\STP20160425.csv
    
###### on linux 
    logstash -f csv\csv2es-stdin.conf < /opt/logstash_2.1.1/bin/csv/data/STP20160425.csv     