# A-HLS Precision Profile Tool Documentation

## Overview

This collection of dashboards, both embedded and stand-alone, provides Sales Reps, Marketing, Product Management, and Leadership with rich insights into facilities and physicians. Sales Reps get insights right in their account and contact pages that are accessible, in-context, and actionable. Others can use the data to understand total-addressable-markets, procedure volumes by sales regions, states, cities, facilities, and physicians. Referral networks can be followed up or down stream to open new opportunities. Combined with internal data this can be extended to understand marketshare and whitespace.

![](/Precision_Profile_Tool/images/preview_ppt_sun.png)

---

## Business Objective

Provide Medical Device sales reps with insights into physician procedure volumes, peer rankings, referral networks, payer mix, and sunshine payments.

## Business Value and Benefits

-    Provides insights for Sales Reps that allows them to tailor their physician engagement, understand their accounts, see the competition, and look for whitespace opportunities.
-    Allows Sales Reps to be more precise with their messaging and spend more time selling, resulting in increased revenue and marketshare.

---

## Industry Focus and Workflow

### Primary Industry:

-    MedTech
-    Medical Sales

### Primary User Persona:

-    Sales Representatives

---

## Package Includes:

### **App Template (1)**

-    Precision Profile Tool App Template

### **Dashboards (8)**

-    ITT Sunshine Payments Dashboard
-    ITT Target Dashboard
-    ITT Payermix Dashboard
-    ITT Network Dashboard
-    ITT Practitioner Network To (Embedded)
-    ITT Practitioner Network From (Embedded)
-    ITT Practitioner (Embedded)
-    ITT Facility (Embedded)

---

## Configuration Requirements

### Pre-Install Configuration Steps:

The following tools must be available and installed:

-    Visual Studio Code
-    An org with Health Cloud installed
     -    Create a text field (255) named `NPI` in both the Account and Contact objects
     -    Create a text field (255) named `SourceSystemId` in both the Account and Contact objects
          -    Select "Do not allow duplicate values", "Treat 'ABC' and 'abc' as duplicate values (case insensitive)"
          -    Select "Set this field as the unique record identifier from an external system"
-    VS Extensions
     -    Salesforce CLI Integration
     -    Salesforce Extension Pack
     -    Salesforce Extension Pack (Expanded)
-    [Install Salesforce CLI](https://developer.salesforce.com/docs/atlas.en-us.242.0.sfdx_setup.meta/sfdx_setup/sfdx_setup_install_cli.htm)
-    Install CLI Analytics plugin by running `sfdx plugins:install @salesforce/analytics`

Please complete the following steps to install the Accelerator:

-    Make sure Dev Hub is enabled in your org
-    Create a Salesforce DX Project in VS Code
     -    Cmd/Ctrl + Shift + P to open Command Palette
     -    Run `SFDX: Create Project`
          -    Ensure the project is fully created with all its folders. The next step to authorize an org will not be available unless this step succeeds.
-    Authorize org in VS Code
     -    Cmd/Ctrl + Shift + P to open Command Palette
     -    Run `SFDX: Authorize an Org` and follow prompts
-    Download the files from https://github.com/healthcare-and-life-sciences/precision-profiling-tool-template, unzip the download, and place the _Precision_Profile_Tool_ folder in your SFDX project in `/force-app/main/default/waveTemplates` (you will need to create the waveTemplates folder).
     -    Specifically, you are copying the "Precision_Profile_Tool" folder from the download into the waveTemplates folder, not the "precision_profiling_tool_template" folder.
     -    NOTE: You don't have to download the folder as noted above if you already downloaded it from the Accelerate HLS site to get here (it's the same thing).

#### Install the Application Template

1. Find the required images in `/waveTemplates/Precision_Profile_Tool/images` and upload them each by going to Setup in your org and searching for "Static Resources" in the Quick Find bar. Click on Static Resources in the left nav, and then click New to upload each image. Make sure to name them exactly the same as the image file name excluding the file type extension. (Ex: “imagename” instead of “imagename.svg”)
     - NOTE: Use the "images" folder insde the "Precision_Profile_Tool" directory, not the "images" folder in the root directory.
2. Deploy template by running `sfdx force:source:deploy -m waveTemplateBundle:Precision_Profile_Tool -u USERNAME` from the project root in VS Code console/command line, where USERNAME is the username you use to log in to your org.
     - NOTE: USERNAME should be the fully qualified name such as "example@myorg.com".

#### Create an App in Analytics Studio

1. For information on how to create an App in Analytics Studio using this template, see this help article: [https://help.salesforce.com/s/articleView?id=sf.bi_templates_create_app.htm&type=5](https://help.salesforce.com/s/articleView?id=sf.bi_templates_create_app.htm&type=5).

---

## Assumptions

1. A customer has licenses for Analytics Studio. These solutions have all been installed and are functional.
2. A customer is assuming Salesforce Lightning Experience — not Classic.
3. Data Model elements that are part of Health Cloud are all available.
4. The Accelerator uses the Lightning Design System standards and look. Customers may want to apply their own branding which can be achieved.

---

## Revision History

-    **Revision Short Description (Month Day, Year)**
     -    Initial (March 22, 2023)
     -    Updated documentation (April 3, 2023)
