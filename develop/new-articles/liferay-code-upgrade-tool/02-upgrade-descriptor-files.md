#LIFERAY CODE UPGRADE TOOL

#UPGRADE DESCRIPTOR FILES 

This page help to upgrade dtd version from 6.2 to 7.0 and delete unused `wap-template-path` tag in descriptor xml files. 

## Overview

(1) Find descriptor files which need to be upgraded

- It shows all files which need to be upgraded when you first switch to the upgrade descriptor files page. Note that you should click on **Find...** button to display the files if you restart liferay code upgrade tool.

![Figure 1: This page displaying all the files which need to upgrade. ](/img/showing-all-the-files.png)

- Double clicking on the file in the list. It will pop up a comparison page which shows the differences between your original source file and the except file.

![Figure 2: The shaded area showing the differences of Source file and Upgrade file. ](/img/comparison-page.png)

(2) Upgrade descriptor files

All the files will be upgraded to 7.0 after clicking on **Upgrade...** button. It will mark the files as `Finished` and change the color of the upgraded files to blue. You also can check if the source file updated to expect by double clicking on one file in the list. 

![Figure 3: The upgraded files name turned to blue. ](/img/upgraded-file-color.png)

(3) Find and upgrade descriptor files again

- Clicking on **Find...** button again, you will find no files need to be upgraded. Besides, there will be a warning message as below:

![Figure 4: The files have already upgrade. ](/img/wraning-message1.png)

- Clicking on **Upgrade...** button again. You will get the below warning message:

![Figure 5: There are no files need to upgrade. ](/img/wraning-message2.png)
