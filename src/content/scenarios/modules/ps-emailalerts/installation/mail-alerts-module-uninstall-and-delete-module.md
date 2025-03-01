---
title: "Mail alerts module - Uninstall and delete module"
weight: 6
---

# Mail alerts module - Uninstall and delete module
## Details
* **Component** : ps_emailalerts
* **Status** : [TEST] To be automated
* **Scenario** : https://forge.prestashop.com/browse/TEST-4128

## Steps
| Step Description | Expected result |
| ----- | ----- |
| Go to BO > Modules > Module manager and search ps_emailalerts | The module page list should be displayed and *Mail alerts* module should be displayed on the list |
| Click on the button at the right of the module > Choose on the list "Uninstall" option | A modal is open with:<br> * *Title*: "Uninstall module?"<br> * *Description*: "You are about to uninstall New products block module. This will definitely disable the module and delete all its files"<br> * *Optional* *checkbox*: "Optional: delete module folder after uninstall."<br> * *Text*: "This action cannot be undone."<br> * *2 buttons*: "Cancel" & "Yes, uninstall it" |
| Click on "Cancel" button or the cross on top right or outside | * The modal is removed<br> * The module list page is displayed |
| Click on the button at the right of the module > Choose on the list "Uninstall" | The modal is open again with the same informations (Title / Description / Optional checkbox / Text / 2 buttons) |
| Check the optional checkbox "Optional: delete module folder after uninstall." > Click on "Yes, uninstall it" button to confirm the uninstallation of the module | * After loading, a green message "Uninstall action on module ps_emailalerts succeeded." is displayed<br> * The module is uninstalled, the button at the right of the module is displaying "Install"<br> * In folders of you shop: yourshop/modules/, the "ps_emailalerts" folder should be removed |
| Click on "View my shop" link in the header > Click on the new tab | The new tab is displayed the FO of the shop with the homepage |
| Scroll down in the homepage and search the "POPULAR PRODUCTS" block > Click on "All products" link | The "Home" category page is displayed |
| Scroll down on this page > Click on the second page of the list > Find your product created (pre-condition) with 0 on quantity > Click on it | * The product page details is displayed<br> * Mail alerts block on the page should be not displayed |
