# derating

此程式將BOM表(.CSV)內的資訊轉成Derating需要的格式並輸出檔案(.CSV)

This program is designed to sort BOM and create a file with every components data in different pages.

Ex.

Input：BOM.csv

Lv|Direct BOM	  |Main Part	  |Rev.	|Seq.	|Part Full Desc.                                                                      |Qty.|Subsitution Part	|Inst. Point	|HSF Property

1	|1395A3078401	|6019B0460301	|A02	|1    |IC,SHUNT REGULATOR,ADJ,SOT-23F,3P,TR                                                 |1   |	-	              |PU895        |	HalogenFree+RoHS2

1	|1395A3078401	|6012B1055302	|A01	|2    |CONNECTOR,POWER CARD EDGE,7.5mm,FL,9A,BLK,50P,2.54mm,90D,PIP,TRAY,LCP,GXT,30U,3.5mm	|2	 |-	                |PJ768,PJ775  |	RoHS2

Output：BOM_output.csv

Page：MicroCircuit

No. |Ref.Desig.	| P/N	        |Component description

1	  |PU895	    |6019B0460301	|IC,SHUNT REGULATOR,ADJ,SOT-23F,3P,T

Page：Connector

No. |Ref.Desig.	| P/N	        |Component description

1	  |PJ768	    |6012B1055302	|CONNECTOR,POWER CARD EDGE,7.5mm,FL,9A,BLK,50P,2.54mm,90D,PIP,TRAY,LCP,GXT,30U,3.5mm

2	  |PJ775	    |6012B1055302	|CONNECTOR,POWER CARD EDGE,7.5mm,FL,9A,BLK,50P,2.54mm,90D,PIP,TRAY,LCP,GXT,30U,3.5mm
