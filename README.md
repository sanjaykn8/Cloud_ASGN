# Cloud Computing Assignment II - local, runnable equivalents

IMPORTANT: I could not retrieve the original notebooks (the S3 links were not reachable, and the
mirrors I found only had the intro text). These scripts are my own local equivalents of each task's
topic, NOT copies of the notebooks. The assignment asks you to run the given notebooks on the
cloud services and show their output - use these scripts to understand/practice the workflow,
but take the screenshots for submission from the real notebooks.

pip install pyspark pandas numpy matplotlib boto3     (Java 8+ needed for Spark)

| Task | Script | Command | Cloud service it stands in for |
|------|--------|---------|--------------------------------|
| 1 Spark Euler  | c1_spark_euler.py | python c1_spark_euler.py [N] | Spark local[*] (same as the notebook) |
| 2 Wikipedia    | c2_wikipedia_explore.py | python c2_wikipedia_explore.py [pageviews file] | AWS EMR |
| 3 CDC data     | c3_datalab_cdc_analysis.py | python c3_datalab_cdc_analysis.py [data.csv] | Google Cloud Datalab |
| 4 Streaming    | c4_kinesis_anomaly.py | python c4_kinesis_anomaly.py [--mode kinesis --stream NAME] | AWS Kinesis |
| 5 SparkML      | c5_sparkml_food_inspection.py | python c5_sparkml_food_inspection.py [Food_Inspections.csv] | Spark MLlib |

Scripts 2, 3 and 5 generate SYNTHETIC data when run without an input file (clearly printed).
Their numbers are invented and must not be reported as real results.
