# Instagram Non-Mutual Followers Identification

Overview

This R script helps identify Instagram users who follow you but do not follow you back. It extracts followers and followings from HTML files, processes the data to find non-mutual followers, and outputs the results into CSV files.

Features

- Extract Usernames: Parses HTML files to extract Instagram usernames.
- Data Processing: Identifies users you follow who do not follow you back.
- Output: Saves results to CSV files and prints them to the console.

How It Works

1. Install and Load Packages:
   - 'rvest': For web scraping HTML files.
   - 'dplyr': For data manipulation.

2. File Paths:
   - Specify the paths to your HTML files containing followers and followings.

3. Extract Usernames:
   - Reads HTML files and extracts Instagram usernames using the `extract_usernames()` function.

4. Data Conversion:
   - Converts the lists of usernames into data frames.

5. Save to CSV:
   - Saves data frames of followers and followings to CSV files.

6. Identify Non-Mutual Followers:
   - Compares lists to find users who follow you but do not follow you back.

7. Output Results:
   - Saves the list of non-mutual followers to a CSV file.
   - Prints the list of non-mutual followers and their sorted (alphabetically) version to the console.

Files Created

- `followers.csv`: Contains the list of your followers.
- `followings.csv`: Contains the list of users you are following.
- `not_following_back.csv`: Contains users you follow but who do not follow you back.
- `nfb_az.csv`: Contains non-mutual followers sorted alphabetically.

Prerequisites

- R installed on your machine.
- HTML files with your Instagram followers and followings data.

Usage

1. Update the file paths in the script to point to your HTML files.
2. Run the script in R.
3. Check the output CSV files for the list of non-mutual followers and their sorted list.

License

This project is open-source and available under the MIT License.
