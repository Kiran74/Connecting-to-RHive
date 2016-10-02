# Connecting-to-RHive

#set environment variable JAVA_HOME 
Sys.setenv(JAVA_HOME="/usr/java/jdk1.8.0_60")

# install the R Hive Package
install.packages("RHive")

# Load the R Hive Package
library(RHive)

rhive.init()
rhive.connect(host="",port="",hiveServer2=TRUE,user="",password="",
properties="hive.principal=")

# Provide the database name 
rhive.use.database("Databasename")

# write the query
rhive.query("select * from table") 
