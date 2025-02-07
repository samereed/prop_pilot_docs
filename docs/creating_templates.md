# Creating Templates
Templates are PowerPoint files that use specific markers to indicate where dynamic content should be inserted. Our system recognizes two types of dynamic content: variables and tables.

# Variables
Variables are marked within slides using double curly braces {{ variable_name }}. These can be placed anywhere in your presentation where you want dynamic content to be inserted. There are three types of variables:

??? "Base variables"
    ### Base variables are written in your .PPTX slides using the {{ variable_name }} syntax. When in doubt, use this type of variable.

    ![Alt text](assets/pp_logo.png)

??? "TMP variables"
    ### Template variables are similar to base variables, but you can put placeholder text inside of them. 
    ### These variables use this syntax: { tmp:variable_name ...placeholder text... }
    ### The main difference between base variables and tmp variables is that tmp variables pass a word count to the AI assistant based on the length of the content that is between the curly braces.

??? "bullet points (experimental)"
    ### Bullet points are specified with the syntax {{ bts:variable_name ...placeholder text... }}
    ### You can add extra text inside of the bullet point variable, just like tmp variables.
    **Please note that this is still an experimental option.**

!!! info "Important"
    Please note that it is still a very good idea to specify the maximum and minimum word count for each field when defining them during the template upload process.