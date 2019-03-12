# Hbase.examples

Let's create an HBase table (emp_details) with below details via Hbase CLI and Java API.


![image](https://user-images.githubusercontent.com/10238655/54198540-d8c89100-451a-11e9-86eb-cdb0c4b13cda.png)


## Via Hbase CLI 

1. Create table schema 

`Syntax:`
```
create 'table_name', 'Column Family1', 'Column Family2',.... 'Column Familyn'
```
```
create 'emp_details', 'Personal', 'Professional'
```

2. Insert data into table 

`Syntax:`
```
put 'table_name', 'rowid', 'ColumnFamily1:Column1',... 'ColumnFamilyn:Columnn'
```
```
put 'emp_details', '1', 'Personal:name', 'John'
```
*To insert the remaining rows, copy paste the commands mentioned in Insert_data_commands.txtt onto HBase Shell*

3. Get data 

`Syntax:`
```
get 'table_name', 'rowid'
```
```
get 'emp_details', '1'
```

