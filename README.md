# BasketballStats
Basketball Statistics Demo
Created by Jordan Volz (jordan.volz@cloudera.com)

**Status**: Demo Ready

**Use Case**: End-to-end spark workflow: data processing, ad-hoc analytics, and predictive analytics

**Steps**:

1. Open a CDSW terminal and run setup.sh
2. Create a Scala Session and run data-processing.scala
3. Create a Python Session and run analysis.py
4. Return to the Scala Session and run machine-learning.scala
5. When finished, run cleanup.scala in your spark session and cleanup.sh in the terminal

**Recommended Session Sizes**: 4 CPU, 8 GB RAM

**Recommended Jobs/Pipeline**:
`data-processing.scala` --> `analysis.py` --> `machine-learning.scala`

**Notes**: 
1. Raw stats are in `/data`
2. `data-processing.scala` --> data transformations + table creations
3. `analysis.py` --> ad-hoc analysis with pandas
4. `machine-learning.scala` --> Regression analysis with spark mllib
5. Your user will need write access into Hive. 

**Estimated Runtime**: 
`data-processing.scala` --> approx 1 min 
`analysis.py` --> < 1 min 
`machine-learning.scala` --> approx 30 min 

**Demo Script**
http://github.mtv.cloudera.com/foe/BasketballStats/blob/master/BasketballStatsDemoScript.docx

**Related Content**:
http://blog.cloudera.com/blog/2016/06/how-to-analyze-fantasy-sports-using-apache-spark-and-sql/
http://blog.cloudera.com/blog/2016/06/how-to-analyze-fantasy-sports-with-apache-spark-and-sql-part-2-data-exploration/
