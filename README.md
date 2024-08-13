Google Consent Mode lets you control how Google tags function depending on whether users have given consent through tools like Evidon. For example, you can specify if users have agreed to allow cookies for Google Analytics or Ads. Based on this consent, the tags will adjust and only use cookies for the approved purposes. This method provides an alternative to completely blocking scripts when consent isn't given.

# Evidon GCM Template
GTM template for Crownpeak

This template works with Google Tag Manager's Consent APIs to manage consent settings and consent mode. It's available in the Tag Manager Community Template Gallery, making it easy for others to use and implement in their projects.

### Table of contents
- [Evidon clients](#evidon-clients)
- [Developers](#developers)
  * [Loading the template in a test account](#loading-the-template-in-a-test-account)
    + [Creating a new tag](#creating-a-new-tag)
    + [Associating a trigger to a tag](#associating-a-trigger-to-a-tag)
  * [Editing this template](#editing-this-template)
    + [Uploading a template.tpl file](#uploading-a-templatetpl-file)
    + [Updating metadata.yaml](#updating-metadatayaml)
    + [Updating the gallery version](#updating-the-gallery-version)
   
## Evidon clients
The idea behind enabling and using GTM templates is to share with all Didomi clients a proven and more frictionless way to interact with Google Consent Mode. This template allows Didomi's clients to create a tag with a simple upload process, so that their websites have Google Consent Mode enabled.


## Developers

The official GTM documentation regarding templates can be found here
https://developers.google.com/tag-manager/templates

### Loading the template in a test account
To use this Google Tag Manager (GTM) template for the Evidon Consent Management Platform (CMP), you'll need to create a new tag in GTM and link the template to at least one trigger. This setup ensures the template functions correctly within your website's tag management system.

#### Creating a new tag
After logging into your Google Tag Manager account and choosing a workspace (we typically use the Default Workspace for testing), you can start configuring your tags and templates.

1. Create a new trigger using "New" button.

  ![image](https://github.com/user-attachments/assets/c1c94177-9e87-408d-9385-cc2e50f01e71)

 Name this trigger and select "Custom Event" as Trigger type.
 
  ![image](https://github.com/user-attachments/assets/464b8375-7ee1-4343-96d8-4d9bd87a4de8)

 Name the event as "evidonAdvancedGoogleConsent" and save
   ![image](https://github.com/user-attachments/assets/18030e11-fb1a-4735-8897-75c3f89f3b14)


2. Click the "New Tag" button as demonstrated in the interface. This action will open a setup screen where you can configure your new tag within Google Tag Manager.
   
  ![image](https://github.com/user-attachments/assets/a5aae064-f7a4-4abf-9d3d-7e10ae3f51a1)


  Alternatively, you can go to the "Tags" tab and click the "New" button located at the top right corner of the tags table. This will also allow you to start setting up a new tag in Google Tag Manager.
  
  ![image](https://github.com/user-attachments/assets/25527b55-c71c-4b30-aaf8-ca352758fd85)

 If you want to add a GA4 tag then attach "evidonAdvancedGoogleConsent" trigger

3. Give the new tag a meaningful name, such as "Evidon CMP" (as used in this example), and then click on the "Tag Configuration" card to proceed with setting up the tag's details.
   
  ![image](https://github.com/user-attachments/assets/fb4aab15-2875-4155-a3b5-7aa79e4f566a)

3. From that screen you should have access to all the templates in the Community Template Gallery, including the "Evidon CMP" one. Look for it and load it.


4. On the "Tag Configuration" screen, you'll see options to access all the templates in the Community Template Gallery. Find the Evidon template by searching for it in the gallery, and then load it into your Google Tag Manager workspace.

    ![image](https://github.com/user-attachments/assets/55a2412b-872c-4513-a2fc-f73717557a75)

Once the template is loaded, you'll have access to its user interface. Here, you'll find few options.

  a) You'll see a checkbox labeled "Enabled Advanced Google Consent Mode." Checking this box will activate the advanced features for managing user consent and configuring tag behavior.

  ![image](https://github.com/user-attachments/assets/f022f96b-4833-4790-b6f4-f724c75999d0)

       Basic Consent Mode: Adjusts how Google tags work based on user consent for cookies. It offers a simple way to handle consent for essential functionalities like Analytics and Ads without detailed 
       customization.
    
       Advanced Consent Mode: Provides more granular control over how consent is managed and applied. It allows for detailed configuration and integration with various consent management platforms (CMPs), 
       offering advanced options for handling different types of user consent and adjusting tag behavior accordingly.
  b) A text box to enter your Company ID
   ![image](https://github.com/user-attachments/assets/f99ba828-7e80-46c2-882b-d82e4afc2668)

  c) Also, you'll find few checkboxes that allow you to set the default status for Google Consent Mode (GCM) according to your preferences.
    ![image](https://github.com/user-attachments/assets/3cba0201-442d-4db2-b7a8-a29154946af2)


#### Associating a trigger to a tag
We want our tag to trigger on all pages. To do this, follow these steps:

1. Click on the "Triggering" card to choose a trigger so that the tag fires.
  ![image](https://github.com/user-attachments/assets/d6b0cd0e-7fa4-4477-9c82-4dc19589fcbc)


2. Select the "Initialization - All Pages" trigger
  ![image](https://github.com/user-attachments/assets/628587cd-3ef4-419b-917c-a7b743f00593)


3. Save the tag. 
 ![image](https://github.com/user-attachments/assets/21a271f1-820d-4f2a-8723-ae159de115e3)


### Editing this template

#### Uploading a template.tpl file
If you need to load a `template.tpl` of this repo into GTM,

1. Get a copy of this repo on your local environment.

2. Go to the "Templates" tab and click on "New"
 ![image](https://github.com/user-attachments/assets/b5a5e5b8-005e-4bf6-be4c-425ec55ce699)

3. At the top right of the template editor menu, choose "Import"
  ![image](https://github.com/user-attachments/assets/02592693-3ada-4fb1-a324-5ae45c32640b)


#### Updating metadata.yaml

Everytime the `template.tpl` is updated and you would want the Community Template Gallery version to reflect those changes, the `medatada.yaml` file should also be updated. The `sha` value must reference the specific `template.tpl` file that you want to publish. Don't forget to update this value correctly with every new version!

See https://developers.google.com/tag-manager/templates/gallery#metadatayaml

#### Updating the gallery version

After the `metadata.yaml` file has been updated, the gallery version of the template will reflect any changes within 2 to 3 days typically. The template users will be notified of said changes and they will have the option of [automatically update to the latest version.](https://support.google.com/tagmanager/answer/9454109#update)

See https://developers.google.com/tag-manager/templates/gallery
