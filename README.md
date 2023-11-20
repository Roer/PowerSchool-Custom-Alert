# Upload Custom Alert Icon

  

-   Log into Admin
    
-   Go to System → Page and Data Management → Custom Page Management
    
-   Right click on the **images** folder and select upload
    
-   Upload a .png or .gif file 24 x 24 pixels in size.
    

  
  
  

# Create Custom Alert

  

-   Log into Admin
    
-   Go to System → Page and Data Management → Custom Page Management
    
-   Expand the **wildcards** folder
    
-   Right click on the **title_student_end_css.txt** file and select **Create New Page Fragment**
    
-   Enter a name for the fragment and change the Insertion Point to **student.alert**
    
-   In the newly created fragment, enter the following code:
    

`~[if#phalert.~([Students.EXTENSION]FieldName)=1]<img src="/images/alert_icon.gif" height=24 width=24 title="Alert Title">[/if#phalert]` 

  

-   Modify the **Students.EXTENSION** to the table that contains the field you wish to alert on (Following a Database.EXTENSION format, i.e. Students.ACTIVITIES)
    
-   Modify **FieldName** to the field you wish to alert on
    
-   Modify **=1** to the conditions for the alert
    
-   Modify /images/**alert_icon.gif** to your alert icon
    
-   Modify **Alert Title** to the text you wish to display on hover
    

  

Follow the same instructions, but with the **teachers_title_student_end_css.txt** wildcard to have the alert show on PowerTeacher
