# AWS-AuroraDBUpgrade

Error :  Getting below error while upgrading aws aurora DB upgrade from aurora mysql 5.7 to Aurora mysql 8.0


Resolution :

1. Create the parameter group  with the default aurora 8.0 and change the **lower_case_table_names** = 1
2. Update  the parameter group name  while upgrading aurora.

   Reference : https://stackoverflow.com/questions/55544132/can-not-create-a-new-rds-mysql-db-instance-with-lower-case-table-names-1
