# upload-metagenomes-to-ncbi
This repo is for demostrating how to archive metagenomic reads in NCBI. 

### Light data submission (BioProject and BioSample)
1. First, you need to login [submission portal](https://submit.ncbi.nlm.nih.gov/?logout_from=%2F) (gmail account will do if you are too lazy to create a new account).

![login submission portal](./images/login_page_submission_portal.png "login submission portal")

2. Once you logged in, click in "My submissions".

![click in my submissions](./images/click_in_my_submissions.jpg "click in my submissions")

3. Now, we start registering a BioProject by clicking in "BioProject" in "Start a new submission" window.
![register a new BioProject](./images/click_in_BioProject.jpg "reigister a new BioProject")

4. To officially start registering a new BioProject, you need to click in "New submission" again.
![further click in new submission for BioProject](./images/further_click_newsubmission.jpg "further click in new submission for BioProject")

5. All sections required for BioProject submission have been unfolded as below using a mock project, you can prepare relavent information accordingly.

![BioProject info combined](./images/bioproject_info_combined.jpg "BioProject info combined")

6. Click in BioSample
![Click in BioSample](./images/click_in_BioSample.jpg "Click in BioSample")

7. Download the batch submission table
![Download batch submission table](./images/download_batch_submission_tab.jpg "Download batch submission table")
![Choose the right table](./images/download_batch_submission_tab2.jpg "Choose the right table")
You can download in the format of either Excel or TSV, below is an example:
![Batch example table example](./images/batch_submission_table_example.jpg "Batch example table example")
You can fill out the form and save it locally for the later use.
8. All sections required for BioSample submission have been unfolded as below, you can prepare relavent information accordingly.
![submitter](./images/BioSample_figure1.jpg "submitter")
![general information](./images/BioSample_figure2.jpg "general information")
![sample type](./images/BioSample_figure3.jpg "sample type")
![attributes](./images/BioSample_figure4.jpg "attributes")
The last section "Review & Submit" is skipped because you will find it very intuitive once you click in.

### Heavy data submission (SRA)
![Click in SRA](./images/click_in_SRA.jpg "Click in SRA")
For archiving heavy data (i.e. SRA), we usually need to preload SRA via FTP.
![FTP upload](./images/FTP_upload.jpg "FTP upload")

CAUTION: If your data is very large (e.g. metagenomic samples), I strongly suggest to use FPT command lines to transfer data. Please visit [How to Use Linux FTP Command to Transfer Files](https://linuxize.com/post/how-to-use-linux-ftp-command-to-transfer-files/) for more details.

You can click "New submission" once the pre-uploading is finished.
![Click new submission](./images/sra_newsubmission.jpg "Click new submission")
![submitter](./images/SRA_figure1.jpg "submitter")
![general info](./images/SRA_figure3.jpg "general info")
![SRA metadata](./images/SRA_figure2.jpg "SRA metadata")
Here you can see the example table:
![metadata example](./images/sra_submission_table_example.jpg "metadata example")
![files](./images/SRA_figure4.jpg "files")

Congratulations! You already uploaded all esstenial components to NCBI for a metagenome project.
If the submission is finally processed successfully, you will see all your submissions being processed like below:
![submission list](./images/submission_list.jpg "submission list")