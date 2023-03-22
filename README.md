![](/Precision_Profile_Tool/images/preview_ppt_sun.png)

# A-HLS Precision Profile Tool Documentation

## Overview

This collection of dashboards, both embedded and stand-alone, provides Sales Reps, Marketing, Product Management, and Leadership with rich insights into facilities and physicians. Sales Reps get insights right in their account and contact pages that are accessible, in-context, and actionable. Others can use the data to understand total-addressable-markets, procedure volumes by sales regions, states, cities, facilities, and physicians. Referral networks can be followed up or down stream to open new opportunities. Combined with internal data this can be extended to understand marketshare and whitespace.

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

### User Workflow:

-    Add
-    Add

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

-    Visual Studio Code
-    An org with Health Cloud installed
     -    Create a text field named `NPI` in both the Account and Contact objects
-    VS Extensions
     -    Salesforce CLI Integration
     -    Salesforce Extension Pack
     -    Salesforce Extension Pack (Extended)
-    [Install Salesforce CLI](https://developer.salesforce.com/docs/atlas.en-us.242.0.sfdx_setup.meta/sfdx_setup/sfdx_setup_install_cli.htm)
-    Install CLI Analytics plugin by running `sfdx plugins:install @salesforce/analytics`
-    Create a Salesforce DX Project in VS Code
-    Make sure Dev Hub is enabled in your org
-    Authorize org in VS Code
     -    Cmd/Ctrl + Shift + P to open Command Palette
     -    Run `SFDX: Authorize an Org` and follow prompts
-    Download Precision_Profile_Tool folder from https://github.com/healthcare-and-life-sciences/precision-profiling-tool-template and place the folder in your SFDX project in `/force-app/main/default/waveTemplates` (you will need to create the waveTemplates folder).

#### Install the Application Template

1. Find the required images in `/waveTemplates/Precision_Profile_Tool/images` and upload them each into Static Resources in your org. Make sure to name them exactly the same as the image file name excluding the file type extension. (Ex: “imagename” instead of “imagename.svg”)
2. Deploy template by running `sfdx force:source:deploy -m waveTemplateBundle:Precision_Profile_Tool -u USERNAME` from the project root in VS Code, where USERNAME is the username you use to log in to your org.

---

## Assumptions

1. A customer has licenses for Health Cloud, Analytics Studio and the HINS Managed Package with OmniStudio. These solutions have all been installed and are functional.
2. A customer is assuming Salesforce Lightning Experience — not Classic.
3. Data Model elements that are part of the HINS (Vlocity) Managed package and Health Cloud are all available.
4. The Accelerator uses the Lightning Design System standards and look. Customers may want to apply their own branding which can be achieved.

---

## Revision History

-    **Revision Short Description (Month Day, Year)**
     -    Initial (March 22, 2023)
