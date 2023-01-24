# Module 04 - Workflows

[< Previous Module](../Modules/module03.md) - **[Home](../README.md)** 


## 1. Upload Notebook
1. Download the [Baby Names Data notebook](../Notebooks/Baby%20Names%20Data.dbc) from the Notebook folder. 
2. In Databricks go to the Workspace tab and select your user name.

    ![Import Notebook](../Images/Module04/importnotebook.png)

3. A screen will appear for you to navigate to the .dbc file you downloaded from step 1. Then select Import.

    ![Upload Notebook](../Images/Module04/uploadnotebook.png)

4. The new notebook should appear in your Workspace. 

**OPTIONAL** You can run through the cells in the notebook if you would like, otherwise move onto the next step.

## 2. Create Job
1. Go to the left hand navigation and select Workflow.

    ![Open Workflows](../Images/Module04/workflow.png)
2. Select Create Job.
3. First you will need to Name your Task. Below are the items you need to input:
    * Task name: Baby_Name_Job
    * Type: Notebook
    * Source: Workspace
    * Path: When you select the path location, go to where you just imported that .dbc file.
    * Cluster: Databricks Lab Cluster (the cluster we created in Module 01)

Then select Create.

![Task Details](../Images/Module04/tasksetup.png)

4. In the top right corner, Select Run Now.
5. Toggle to the Run view of the job. It should only take about 10 seconds for a Successful Run to appear.

    ![Successful Run](../Images/Module04/successfulrun.png)

6. Select the successful runs log time to view the output. It will show you the code run in the cells and the output of the queries.

    ![Output of Successful Run](../Images/Module04/outputtask.png)

**Note** If you ran this code in the notebook, you will have the same output.

## 3. Run with Different Parameters
1. Open the Baby_Name_Run Job and select the dropdown next to Run now. Select Run now with different parameters.

    ![Run Different Parameters](../Images/Module04/diffparameters.png)

2. Under UI, we will add the year 2015 to filter our names on.
    * Key: year
    * Value: 2015

    Then select Run

    ![Run New Task Parameters](../Images/Module04/runnewparam.png)

3. After a successful run, open the logs again to see the output. Even though the cell says it is filtering on 2014, the results show 2015 due to the different parameters being passed.

    ![Run New Task Parameters 2015](../Images/Module04/2015output.png)