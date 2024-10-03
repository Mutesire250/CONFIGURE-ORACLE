# CONFIGURE-ORACLE
JUST CONFIGURATION

Connecting to the Database:

This part indicates that you are logging into the Oracle database as a user with DBA (Database Administrator) privileges (sysdba). This is necessary for creating and managing pluggable databases (PDBs).
2.	Creating a Pluggable Database (mu_plsqlauca):

o	CREATE PLUGGABLE DATABASE: This command initiates the creation of a new PDB named mu_plsqlauca.
o	ADMIN USER: It creates an administrative user for the PDB named mu_plsqlauca with the password mutesire.
o	FILE_NAME_CONVERT: This parameter helps in converting the file names from the seed PDB (which serves as a template) to the new PDB. It specifies the original location of the seed's data files and where the new PDB's data files should be located.
o	DEFAULT TABLESPACE users: This specifies that the default tablespace for the new PDB will be named users.
o	DATAFILE: This specifies the path and size for the initial data file for the default tablespace. It creates a data file named users01.dbf with a size of 250 MB that can auto-extend as needed.
3.	Creating Another Pluggable Database (mu_to_delete_plsqlauca
o	This command follows the same structure as the previous one, creating another PDB named mu_to_delete_plsqlauca with similar parameters and a corresponding data file.
4.	Dropping a Pluggable Database (mu_to_delete_plsqlauca):
o	DROP PLUGGABLE DATABASE: This command removes the PDB named mu_to_delete_plsqlauca from the database.
o	INCLUDING DATAFILES: This option ensures that the associated data files are also deleted from the file system, freeing up space.
Summary:
•	You successfully created two pluggable databases, each with an admin user and specified file paths.
•	You also dropped one of the created pluggable databases along with its data files, demonstrating database management operations in an Oracle multitenant architecture.

![Screenshot 2024-10-03 201447 one](https://github.com/user-attachments/assets/ab0c3080-3159-4d22-aa78-0cb5e2f1f45d)
![Screenshot 2024-10-03 201620  two](https://github.com/user-attachments/assets/8a8510db-5642-4e5e-866e-871dd90ba569)
![divinejpp](https://github.com/user-attachments/assets/c66f6e3f-9637-4b82-91b3-9c2999533a36)








