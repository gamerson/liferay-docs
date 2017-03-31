#LIFERAY CODE UPGRADE TOOL

#FIND BREAKING CHANGES 

This page helps you to find breaking changes of java, jsp, xml and properties files. It will not support to find the front-end codes(e.g., javasript, css).

To see more about breaking changes, please refer to [Breaking Changes for Liferay 7.0](https://github.com/liferay/liferay-portal/blob/master/readme/7.0/BREAKING_CHANGES.markdown).

## Overview

Besides the description and six buttons at the right of the view, it's blank by default. 

![Figure 1: Switch to Find Breaking Changes pages, showing blank by default.](/img/find-breaking-changes-first-page.png)

What are the buttons mean:

- **Find Breaking Changes:** Find breaking changes problems.
- **Automatically Correct Problems:** Correct problems automatically .
- **Expand All:** Expand the project tree.
- **Collapse All:** Collapse the project tree.
- **Open Ignored List:** Go to migration problem.
- **Hide Tree:** Hide the tree and display the guidelines only.

## How to resolve breaking change problems? 

(1). Clicking on `Find Breaking changes` button.

![Figure 2: When selecting *Find Breaking Changes* &rarr; *Select or Deselect* &rarr; *OK*, all the problems will be found.](/img/find-breaking-changes-button.png)

(2). Select or deselect projects in the pop up 'Project Selection' dialog.

(3). Clicking on OK button. You are able to see 'Code Problems' tree in the upper-left corner once finish finding breaking changes.

(4). Expand all.

(5). Clicking on the specific file. You can see the problems and contextual documentation.

![Figure 3: You can fix problems according to the guidelines.](/img/find-breaking-changes-problems-page.png)

(6). Resolve the problems according to the contextual documentation.

## Dealing with problems

(1). In problem tab, there are three columns as below:

 - **Resolved:** You can mark the problem as resolved.
 - **Line:** Show line numbers and you can arrange them in ascending or descending order.
 - **Problem:** Show problems.
 
(2). Options when right clicking on a problem

 - **Mark done:** Make the checkbox of the problem as resolved. If you haven't change the code and mark it as resolved, it will show up when finding break changes again.
 - **Mark undone:** Unchecked the checkbox.
 - **Ignore:** Ignore the problem.
 - **Correct automatically:** Correct the selected problem automatically.
 - **Ignore all problems of this type:** Ignore all problems of this type.

![Figure 4: Right click on the problem, you are giving five options of this problem.](/img/correct-automatically.png)

   Correct problems automatically:
 
 - Right clicking on a specific problem to check if it is allowed to `Correct automatically`. 
 - Besides, all the problems which are allowed to correct automatically can be resolved concurrently by clicking on the button `Automatically Correct Problems`.
 - Clicking on `Find Breaking Changes` again, you will find that all the allowed auto correct problems are no longer exist.
 
   Ignore all problems of this type:

 - Right click on the problem and select the option *Ignore all problems of this type*,  all the same type of this problem will be ignored.
 - Go to **Open Ignored List** to check the ignored details.
 - Find the problems again. You will find that all the ignored problems can't be found now.
 - Remove the ignored problems by selecting the problems &rarr; Remove &rarr; Apply &rarr; OK.

![Figure 6: The removed problems details include *Tickets*, *Problem*, *Detail Information* .](/img/ignore-list-details.png)
 
 
(3). Double clicking on one problem to open it, it will switch to the corresponding line number and show marks. When you resolved this problem, the mark will be removed.

![Figure 5: If the problem resolved , the markdown and red fork will disappear.](/img/markdown.png)

(4). After correcting the problems automatically, you need to resolve the rest of problems manually. Once you resolved all of them, congratulations, you made it.










