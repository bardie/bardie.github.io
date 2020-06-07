---
layout: default
---

# Operations Cheat Sheet

## Import Libraries

### Panda

```
 import pandas as pd
```

### Spark

```
from __future__ import print_function
from pyspark.sql.types import StructType, StructField, StringType, IntegerType, ArrayType, TimestampType, DoubleType
from pyspark.sql.functions import count, date_format, window,  countDistinct, avg, max, explode
from pyspark.sql.window import Window
import pyspark.sql.functions as F
from pyspark.ml import Pipeline
```

### Numpy

```
 import numpy as np
```

## Read and Write Files

### CSV

#### Pandas

```
pd.read_csv( , header=None, nrows=5)
df.to_csv('myDataFrame.csv')
```

#### Spark

```
schema = StructType([StructField("Timestamp", TimestampType(), True),
                         StructField("EventId", IntegerType(), True),
                         StructField("EventType", StringType(), True),
                         StructField("Class", StringType(), True),
                         StructField("SourceIP", StringType(), True),
                         StructField("DestinationIP", StringType(), True),
                         StructField("SourcePort", StringType(), True),
                         StructField("DestinationPort", StringType(), True)])
                         
df = spark.read.csv('/home/test/file.csv', schema=schema, inferSchema=True).sort("Timestamp", ascending=True).na.drop()
```

### Excel

#### Pandas

```
pd.read_excel( )
df.to_excel('dir/myDataFrame.xlsx', sheet_name='Sheet1')
 # Read multiple sheets from the same file
xlsx = pd.ExcelFile( )
df = pd.read_excel(xlsx, 'Sheet1')
```

## Read and Write to SQL Query or Database Table

#### SQLITE

##### Pandas

```
from sqlalchemy import create_engine
engine = create_engine('sqlite:///:memory:')
pd.read_sql("SELECT * FROM my_table;", engine)
pd.read_sql_table('my_table', engine)
pd.read_sql_query("SELECT * FROM my_table;", engine)
```

## References

- https://www.datacamp.com/community/data-science-cheatsheets?posts_selected_tab=must_read&tag=python
