# Understanding File Permissions

## Task 1 --- Create a File

Run:

    touch secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)<img width="1090" height="100" alt="image" src="https://github.com/user-attachments/assets/2690f3d0-111d-4655-a398-efec9bc90d5f" />


### Questions

1.  Who owns the file? I owns the file
   
3.  What are the default permissions? 
The default permissions depend on the file type and system settings. They are commonly:
- Owner: Read and write.
- Group: Read only.
- Others: Read only.
- 
### Reflection

Why is file ownership important in Linux systems?

File ownership is important in Linux because it controls who can access, read, write, or modify files. It helps protect sensitive information, prevent unauthorised access, and keep the system secure.

------------------------------------------------------------------------

## Task 2 --- Restrict File Permissions

Run:

    chmod 600 secret.txt
    ls -l secret.txt

### Screenshot.  -rw-------

(Add screenshot here)<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/4ecefa13-6cc9-424e-b672-5e42a1d63856" />


### Questions

1.  Who can read the file now?
   just the owner
3.  Who cannot access it?
anyone else

------------------------------------------------------------------------

## Task 3 --- Open Permissions (Security Risk)

Run:

    chmod 777 secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/bbdbd114-65be-4f95-af72-ece64fcece4c" />


### Questions

1.  Who can access the file now? everybody
2.  Why might this configuration be dangerous? becouse everyone can access the file and change it.

