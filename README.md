# hadoop-c06p195

## hadoop Map Reduce Programming 

### dhdhdh
    chapter06
    page 195
    
    	예제 데이터(아파치 로그): http://ita.ee.lbl.gov/html/contrib/NASA-HTTP.html
		wget ftp://ita.ee.lbl.gov/traces/NASA_access_log_Jul95.gz
	  768  hadoop fs -mkdir input02
	  769  hadoop fs -put NASA_access_log_Jul95 input02
	  770  hadoop fs -lsr input02
	  771  hadoop jar Chapter06p195-0.0.1-SNAPSHOT.jar p195.WebLogMessageSizeAggregator input02 output02
	  772  hadoop fs -lsr output02
	
	[icarus@cent1 PDM]$ hadoop fs -cat output02/part-r-00000
		Mean    1150
		Max     6823936
		Min     0