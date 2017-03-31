# Liferay Code Upgrade Tool

# Custom Jsp Page

This page helps you convert your projects with custom jsp hooks to modules or fragments.

![Custom Jsp](images/customJsp.png)

## 1 Converted Project Location:

This field will show your projects location by default. You could also click `Browse...` button to browse your project location that you want to convert.

Location can't be empty:

![Converted Location is empty](images/locationEmptyMessage.png)

## 2 Select Projects

When clicking on `Select Projects` button, it will pops up a dialog with all available custom jsps hook projects that you are able to convert. 

![Select Projects](images/selectProjects.png)

You could click `Select All` button or `Delete All` button to select all projects for converting or delete all projects now needn't to convert. Or you could also select one or more projects you want to convert by clicking checkbox.

Click `OK` button when you finish selecting projects. The result will looks like the following.

![result](images/result.png)

## 3 More actions:

1) Checking which jsp hooks can be found. It can't be found if it's defined by yourself.

![jspHookBeFound](images/jspHookBeFound.png)

2) Double clicking on the jsp file in both '6.2 Custom JSPs' and 'New JSP' columns to see more details.  

Double-click the jsp file that compare with 6.2:

![double-click the jsp file that compare with 6.2](images/compareWith6.2.png)

Double-click the jsp file that compare 6.2 with 7.x:

![double-click the jsp file that compare 6.2 with 7.x](images/compare6.2With7.x.png)

3) `Refresh Results` Refresh results.

4) `Clear Results` Clear results.

## 4 Notes:

When you want to convert again after finish converting projects, you have to delete the converted projects from disk. Otherwise, you will run into an error.

