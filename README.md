# Database_Creation_Deletion_of_PDBs-Pluggable_Database-

## Tasks Completed
1. Created a Pluggable Database (PDB) named `plsql_class2024db`.
2. Created and deleted a temporary PDB named `ne_to_delete_pdb`.
3. Configured Oracle Enterprise Manager

## SQL Commands Used

 ## Create plsql_class2024db
 -This command creates a new Pluggable Database (PDB) named `plsql_class2024db` with an admin user named 'ne_plsqlauca'.
 
 CREATE PLUGGABLE DATABASE plsql_class2024db 
ADMIN USER ne_plsqlauca IDENTIFIED BY password 
FILE_NAME_CONVERT = ( 'C:\app\NELYSE\product\21c\oradata\XE\pdbseed\',  'C:\app\NELYSE\product\21c\oradata\XE\XEPDB1\plsql_class2024db\');
ALTER PLUGGABLE DATABASE plsql_class2024db OPEN;

 ## Create ne_to_delete_pdb
 -This command creates a temporary Pluggable Database (PDB) named ne_to_delete_pdb with an admin user named 'ne_plsqlauca'.
 
 CREATE PLUGGABLE DATABASE ne_to_delete_pdb 
ADMIN USER ne_plsqlauca IDENTIFIED BY password 
FILE_NAME_CONVERT = ( 'C:\app\NELYSE\product\21c\oradata\XE\pdbseed\',  'C:\app\NELYSE\product\21c\oradata\XE\XEPDB1\/ne_to_delete_pdb/');
ALTER PLUGGABLE DATABASE ne_to_delete_pdb OPEN;

 ## Delete ne_to_delete_pdb
 -This command deletes the temporary PDB ne_to_delete_pdb and includes its data files

 DROP PLUGGABLE DATABASE ne_to_delete_pdb INCLUDING DATAFILES;

## Screenshots

1.This is the screenshot of Creating pluggable database named 'plsql_class2024db'.

![plsql_class2024db](https://github.com/user-attachments/assets/92509100-58bd-401a-a22c-47d2d7293ee4)

2.This is the screenshot of Creating a temporary pluggable database named 'ne_to_delete_pdb'.

![ne_to_delete_pdb](https://github.com/user-attachments/assets/8d739c6a-5b5c-4804-ae23-f716467b5a1c)

3.This is the screenshot of deleting a temporary  pluggable database named 'ne_to_delete_pdb'.

![delete_ne_to_delete_db](https://github.com/user-attachments/assets/888c590f-b6f4-4ce1-8f89-83dbb257d283)

4.This is the screenshot of checking if the 'ne_to_delete_pdb' Dropped successfully.

![check_if_pdb_is_dropped](https://github.com/user-attachments/assets/f43245cd-9ffa-4ff4-b2f2-d3fbce84fdf8)

5.This is the screenshot of 'Oracle Enterprise Manager Dashboard'.

![SAMPLE_DASHBOARD](https://github.com/user-attachments/assets/753eaad7-d161-4f3f-b3fd-7a510fb6cd70)


                                                           
                                                           
                                                                     
                                                                     ## Done by Nelyse!!!!



