# Lab 7: Practice with Selenium

### Instructions - please read and follow carefully
* *Accept the Assignment*: When you accept the assignment in GitHub Classroom, a repository named `lab-07` will be automatically generated for you under the "s386Fall2023" organization.
* *Locate Your Repository*: Your personal repository for this homework can be found at `https://github.com/s386Fall2023/lab-07-your_user_name`.
* *Clone the Repository*: 
    - Open your terminal and navigate to the directory where you want to download the repository.
    - Run `git clone your_repository_URL` to clone the repository onto your local machine.
* *Working Directory*: The cloning process will create a new directory named `lab-07-your_user_name`. Ensure that you perform all your work inside this directory.
* *Commit Your Progress*: As you work on the assignment, remember to commit your changes periodically. You can easily do this using Visual Studio Code (VS Code).
* *Remote Connection*: If you've cloned the repository correctly and are working within the created directory, the remote link to your GitHub repository should already be configured.
* *File and Function Names*: 
    - Upload the code you used to complete the file and the requests csv (the `audiobooks.csv` file) to the repository
* *Virtual Environment*: Ensure that you are using the class's virtual environment while working on this assignment.
   - Note:  There is no way to tell from your submission whether or not you use the class environment.  However, if you are working in the virtual environment set up for our class, then you can be sure that you are using the correct versions of the packages.
* *Submitting on Gradescope*: 
    - Once you've completed the assignment, go to Gradescope and select your personal homework repository (`https://github.com/s386Fall2023/lab-07-your_user_name`) as the source for your submission.
    
    
-----
## Instructions

For this homework assignment you will practice web scraping using Python and Selenium to extract data from the Audible.com website. In this assignment, you will write a Python script to scrape information books on Audible.com and then analyze and present the data in a structured format.


1.  Update Selenium if you haven't already done so:
```bash
# in terminal with class environment activated
conda install -c conda-forge selenium=4.14
```
2. Install webdriver-manager if you haven't already done so:
```bash
# in terminal with class environment activated
pip install webdriver-manager
```
3.  Using Selenium, create a DataFrame of the [bestselling](https://www.audible.com/adblbestsellers?ref_pageloadid=h7Ag5cGcQ5yvRAVu&ref=a_search_b1_desktop_footer_column_2_0&pf_rd_p=6a55a63d-48d3-4d5e-857f-ae6682380e4d&pf_rd_r=65QXM553SAAQNRH2VDV2&pageLoadId=yGFSdjIrgVpQDcAP&ref_plink=not_applicable&creativeId=2d835e86-1f10-4f6e-a4c6-33d2001684e6) audio books on audible.

Your DataFrame should have 100 rows and 5 columns:

| title | author | runtime | release_date | list_number |
|-------|------|-------|------|----------|
|*title*|*author*|*runtime*|*release_date*|*list_number*| 

where 
- "title" is the book title, 
- "author" is author of the book 
- "runtime" is the length of the audio book
- "release_date" is the release date of the audio book
- "list_number" is the number that the audio book appears on the list

4.  Save your DataFrame as a `.csv` file called `audiobooks.csv` and commit it to your repository
