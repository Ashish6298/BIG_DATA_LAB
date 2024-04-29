## Steps to run the program:-

## Create a folder of ypur name or usn. 

## Now Open the terminal and type the following commands.

```bash
start-all.sh
```

```bash
jps
```


```bash
hadoop version
```


```bash
javac -version
```

## Now create 2 folder "inputdata" and "javaclass" in the same folder where you created the above folder.

## Now go inside the "inputdata" folder by typing "cd inputdata" in the terminal and create a new textfile of any name for example "1.txt".

## Now write anything in that text file.

## now comeback to the your original directory by typing " cd .. " .

## Now type the following commands again.

```bash
export HADOOP_CLASSPATH=$(hadoop classpath)
```

```bash
echo $HADOOP_CLASSPATH
```

```bash
hadoop fs -mkdir /wordcount
```

```bash
hadoop fs -mkdir /wordcount/Input
```

## Now open browser and type "localhost:9870"

## A website will open where u can see the uploads of your data. Initially it will be empty so follow these commands to insert the data.

```bash
hadoop fs -put ./inputdata/1.txt/ /wordcount/Input
```
## OR


*hadoop fs -put (drag and drop the file it will take the path automatically) and then add "/wordcount/Input"*


