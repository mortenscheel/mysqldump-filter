# mysqldump-filter
A CLI tool that allows filtering out data from selected tables in a .sql dump.

## Installation
```shell
composer global require mortenscheel/mysqldump-filter
```

## Usage
Example:
```shell
cat dump.sql | mysqldump-filter --skip=some_table,another_table | mysql -u username -p db_name

cat dump.sql | mysqldump-filter --only=some_table,another_table | mysql -u username -p db_name
```

## Contributions
All contributions are welcome