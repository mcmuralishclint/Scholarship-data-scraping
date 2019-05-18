# China Scholarship Data
A project to create a cleaned dataset from the scholarship data collected from https://www.cucas.edu.cn/china_scholarships/

## Part 1 - Web Scraping

The scholarship data was scraped from a leading educational consultancy.

**How does it work?**

- The scholarships are divided into 4 types: Non-degree, Bachelors, Masters and PhD. I used this information to navigate through pages.
- Each scholarship type is taken and the total number of scholarships for each type is found which is displayed at the bottom of the page.
- 15 scholarships are displayed on a page and the total number of pages can be found by dividing the total scholarships by 15. If the result is a whole number, The number of pages will be the result and otherwise the result will be result plus 1
- The majors, titles, language of instruction, tuition fees to pay, tuition fees to covered are scraped from the website.
- Some string manipulation is used to extract data which are not in the usual format.

## Part 2 - Data Cleaning

The scraped data was very untidy and contained many un-clean data. 
