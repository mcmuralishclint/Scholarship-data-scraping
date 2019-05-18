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
The whole project was divided into 7 parts.

- PART 1-Convert start date to two columns (Month, Year)
- PART 2-Convert the contents of the field Tuition Covered (Data in the Tuition field are stored in different formats. Some of them are integers and most of them have commas, words, '-''s etc)
- PART 3-Convert the contents of the field Accomodation Covered (Data in the Accomodation field are stored in different formats. Some of them are integers and most of them have commas, words, '-''s etc)
- PART 4-Convert the contents of the field Living expense Covered (Data in the Living expense field are stored in different formats. Some of them are integers and most of them have commas, words, '-''s etc)
- PART 5-Convert tuition fees, original tuition fees to pay to currency (RMB) 
- PART 6-Convert Accomodation to pay to two fields (Accomodation price, Accomodation duration)
- PART 7-Convert Living expense to pay to two fields (living expense , living duration)
