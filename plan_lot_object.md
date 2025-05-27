# Plan for Creating Custom Object 'Lot'

## 1. Create Custom Object 'Lot'
    - **File Path:** `force-app/main/default/objects/Lot__c/Lot__c.object-meta.xml`
    - **Short Description:** Defines the custom object 'Lot', its basic properties, and a default Search Layout.
    - **Cursor rule that applies:** `custom-object.mdc`
    - **sfdx command used to deploy:** `sfdx force:source:deploy -p "force-app/main/default/objects/Lot__c/Lot__c.object-meta.xml"`

## 2. Create Compact Layout for 'Lot'
    - **File Path:** `force-app/main/default/objects/Lot__c/compactLayouts/Lot_Compact_Layout.compactLayout-meta.xml`
    - **Short Description:** Defines the compact layout for the 'Lot' object, to be stored within the object's own folder.
    - **Cursor rule that applies:** `compact-layout.mdc`
    - **sfdx command used to deploy:** `sfdx force:source:deploy -p "force-app/main/default/objects/Lot__c/compactLayouts/Lot_Compact_Layout.compactLayout-meta.xml"`

## 3. Create Page Layout for 'Lot'
    - **File Path:** `force-app/main/default/layouts/Lot__c-Lot Layout.layout-meta.xml`
    - **Short Description:** Defines the page layout for the 'Lot' object.
    - **Cursor rule that applies:** `page-layout.mdc`
    - **sfdx command used to deploy:** `sfdx force:source:deploy -p "force-app/main/default/layouts/Lot__c-Lot Layout.layout-meta.xml"`

## 4. Create Custom Tab for 'Lot'
    - **File Path:** `force-app/main/default/tabs/Lot__c.tab-meta.xml`
    - **Short Description:** Creates a custom tab for the 'Lot' object to make it accessible in the Salesforce UI.
    - **Cursor rule that applies:** `custom-tab.mdc`
    - **sfdx command used to deploy:** `sfdx force:source:deploy -p "force-app/main/default/tabs/Lot__c.tab-meta.xml"`

## 5. Create Lightning Record Page for 'Lot'
    - **File Path:** `force-app/main/default/flexipages/Lot_Record_Page.flexipage-meta.xml`
    - **Short Description:** Defines the Lightning Record Page for the 'Lot' object.
    - **Cursor rule that applies:** `lightning-record-page.mdc`
    - **sfdx command used to deploy:** `sfdx force:source:deploy -p "force-app/main/default/flexipages/Lot_Record_Page.flexipage-meta.xml"`

## 6. Create Object Level Permission Set for 'Lot'
    - **File Path:** `force-app/main/default/permissionsets/Lot_Object_Permissions.permissionset-meta.xml`
    - **Short Description:** Defines a permission set for object-level access to the 'Lot' object (e.g., Read, Create, Edit, Delete).
    - **Cursor rule that applies:** `permission-sets.mdc`
    - **sfdx command used to deploy:** `sfdx force:source:deploy -p "force-app/main/default/permissionsets/Lot_Object_Permissions.permissionset-meta.xml"`

## 7. Create Field Level Permission Set for 'Lot'
    - **File Path:** `force-app/main/default/permissionsets/Lot_Field_Permissions.permissionset-meta.xml`
    - **Short Description:** Defines a permission set for field-level security for the 'Lot' object's fields. Initially, this will be basic as we haven't defined custom fields yet beyond standard ones.
    - **Cursor rule that applies:** `permission-sets.mdc`
    - **sfdx command used to deploy:** `sfdx force:source:deploy -p "force-app/main/default/permissionsets/Lot_Field_Permissions.permissionset-meta.xml"` 