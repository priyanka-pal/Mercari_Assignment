# Mercari_Assignment :Automating use-case for Mercari site


This project demonstrates a Test Automation Framework built using Selenium WebDriver and TestNG to validate functionalities following use-case:

Scenario 1
Search conditions are set correctly.
Steps:
1. Go to Mercari top page (https://jp.mercari.com/)
2. Click on the search bar
3. Click on "Select by category" (カテゴリーからさがす)
4. Select "Books, Magazines & Comics" as the tier 1 category (本・雑誌・漫画)
5. Select "Books" as the tier 2 category (本)
6. Select "Computers & Technology" as the tier 3 category (コンピュータ/IT)
7. Verify the search conditions on the left sidebar are set correctly

Scenario 2
Search conditions are set correctly from the latest browsing history.
Pre-condition:
Create 2 browsing history entries. The latest one should be the categories in Scenario 1.
(You can create browsing history by following the same steps in Scenario 1)
Steps:
1. Go to Mercari top page (https://jp.mercari.com/)
2. Click on the search bar
2. Verify there are 2 browsing histories
3. Verify the latest browsing history is showing correctly (Computers & Technology / コンピュータ/IT)
4. Click on the latest browsing histories
5. Verify the search conditions on the left sidebar are set correctly
6. Input "javascript" in the search bar and search with the keyword
7. Go back to Mercari top page (https://jp.mercari.com/)
8. Verify there are 3 browsing histories
9. Verify the latest browsing history is showing correctly (javascript, Computers & Technology / javascript, コンピュータ/IT)


Table of Contents
Overview
Project Structure
Test Description
Pre-requisites
Setup and Execution
Test Scenarios
Reporting
Acknowledgments


Overview 
This framework is designed to automate the launch of a web application and validate the above two use-case. Framework is desgined  using Page Object Model (POM) principles, Contains test classes such as TestCase01 to validate specific features.

Implements the Page Object Model (POM) with classes like HomePage and LaunchPage for modularized and reusable web interactions.

URL Launch: Opens the web application at https://jp.mercari.com and verifies that the correct URL is loaded.
Language Change: Switches the application language to English - EN.
Category Search: Navigates to the category search section, selects as per the use-case categories, and verifies the selected search conditions.
Pre-requisites
Install Java 8 or higher.
Install Maven to manage dependencies.
Install Google Chrome and the corresponding ChromeDriver for Selenium.
Add the following dependencies to your pom.xml:
Selenium WebDriver
TestNG









