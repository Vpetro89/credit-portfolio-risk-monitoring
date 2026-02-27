\# DAX Measures



\## Loss Rate



Loss Rate =

DIVIDE(

&nbsp;   SUM(Sheet1\[charge\_off\_flag]),

&nbsp;   COUNT(Sheet1\[loan\_id])

)



\## 30+ Exposure



30+ Exposure =

CALCULATE(

&nbsp;   SUM(Sheet1\[current\_balance]),

&nbsp;   Sheet1\[delinquency\_status] = "30"

)



\## Expected Loss



Expected Loss =

SUMX(

&nbsp;   Sheet1,

&nbsp;   Sheet1\[current\_balance] \* Sheet1\[loss\_rate]

)

