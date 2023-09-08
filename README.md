# Automated Sanction Name Screening RPA at [OpenSanctions](https://www.opensanctions.org)

This repository contains a proof of concept Robotic Process Automation (RPA) project that demonstrates automation technology applied to bulk KYC (Know Your Customer) name screening. The RPA utilizes Power Automate Desktop to perform automated name screening on the [OpenSanctions](https://www.opensanctions.org) website without manual human intervention.

## Overview

The proof of concept design objective was to create an RPA that can perform the following tasks:

- Automated name screening at a website.
- Screenshot no-hits searches.
- Flag names with possible matches into a display message.

## Enhanced Features to PRD

The initial proof of concept was upgraded to a production-grade RPA flow with a total of 116 steps. The enhanced RPA can now achieve the following impressive features:

- Screenshot the first page of the name match list.
- Click the next arrow on the scroll bar.
- Screenshot every subsequent name match listing webpage till the last page.
- Capture all names and the URL links.

For each match, it can:

- Go into the URL Link for each match.
- Click on the '...more' hyperlink to uncover hidden items.
- Screenshot and save the screenshot file named appropriately for easy search in folders.

## Usage

To use this RPA project to automate sanctions screening on [OpenSanctions](https://www.opensanctions.org), follow these steps:

1. **Prerequisites**: 
   - Install [Power Automate Desktop](https://powerautomate.microsoft.com/en-us/robotic-process-automation/) on your PC.

2. **Configuration**:
   - Create a new project in Power Automate Desktop.
   - Follow and create the steps in the pdf file.
   - Configure any necessary settings along the way.

3. **Execution**:
   - Run the RPA flow. It will automate the sanctions screening process on OpenSanctions, capturing relevant screenshots and generating reports.

4. **Reports**:
   - Once the RPA execution is complete, check the generated Excel report for the results.

## Reporting

The RPA generates an Excel report that contains all the names screened, separating the names with no hits from the names with matches. It displays the possible matched names and their URL links side-by-side in adjacent columns.

## Performance

The RPA took 69 minutes to complete a randomly mixed name screening of 18 names, including 9 with no hits and 9 screened names with possible name matches. The duration was extended due to the presence of numerous false name matches (approximately 300 matches) when the screened name returned a long list of false matches.
