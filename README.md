# Learn SQL in a minute
From your local pc, perform git clone https://github.com/jasonwcc/learntosql

# Make sure that you have a database system is running (may refers to Deploying mysql containers lab)

# Create Table with following details:
- user : user1 \
- user password : mypa55 \
- host : ${mysql_ip} \
- database name : items

mysql -uuser1 -pmypa55 -h ${mysql_ip} items < ~/createtable.sql
  
# Insert rows into projects using above details:
mysql -uuser1 -pmypa55 -h ${mysql_ip} items < ~/insertrows.sql
