# Database_Creation_Deletion_of_PDBs-Pluggable_Database-

## Tasks Completed
1. Created a Pluggable Database (PDB) named `plsql_class2024db`.
2. Created and deleted a temporary PDB named `ne_to_delete_pdb`.
3. Configured Oracle Enterprise Manager.

## SQL Commands Used

### Create plsql_class2024db
```sql
CREATE PLUGGABLE DATABASE plsql_class2024db 
ADMIN USER ne_plsqlauca IDENTIFIED BY password 
FILE_NAME_CONVERT = ( 'C:\app\NELYSE\product\21c\oradata\XE\pdbseed\',  'C:\app\NELYSE\product\21c\oradata\XE\XEPDB1\plsql_class2024db\');
ALTER PLUGGABLE DATABASE plsql_class2024db OPEN;

## Create ne_to_delete_pdb

CREATE PLUGGABLE DATABASE ne_to_delete_pdb 
ADMIN USER ne_plsqlauca IDENTIFIED BY password 
FILE_NAME_CONVERT = ( 'C:\app\NELYSE\product\21c\oradata\XE\pdbseed\',  'C:\app\NELYSE\product\21c\oradata\XE\XEPDB1\/ne_to_delete_pdb/');
ALTER PLUGGABLE DATABASE ne_to_delete_pdb OPEN;

## Delete ne_to_delete_pdb

DROP PLUGGABLE DATABASE ne_to_delete_pdb INCLUDING DATAFILES;

## Screenshots
1.This is the screenshot of Creating pluggable database named 'plsql_class2024db'.


2.This is the screenshot of Creating a temporary pluggable database named 'ne_to_delete_pdb'.


3.This is the screenshot of deleting a temporary  pluggable database named 'ne_to_delete_pdb'.


4.This is the screenshot of 'Oracle Enterprise Manager Dashboard'.
