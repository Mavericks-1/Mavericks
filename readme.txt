Menu Creation in Drupal: Content Menu and Self-Service Menu
As part of enhancing the site's navigation, we are creating two new custom menus within Drupal:

Content Menu:

Purpose: The Content Menu will serve as a central navigation tool for managing and organizing content across the site. This menu will allow administrators to configure menu lists and pages that are directly related to content navigation. It will streamline access to various content types, making it easier for users to find and manage the content they need.

Usage: This menu is particularly useful for site administrators and content managers who need to organize the website’s content structure effectively. It can be used to group content types, categories, and individual content items into a logical and user-friendly hierarchy.

Self-Service Menu:

Purpose: The Self-Service Menu is designed to provide users with a clear and intuitive pathway to access their self-service pages. This menu will include links to user-specific pages such as profile management, account settings, and other personal user tools.

Usage: This menu is intended to improve user experience by offering a streamlined navigation option for users to manage their accounts and access personalized services. It will be primarily accessible to authenticated users, offering them a convenient way to manage their interactions with the site.






Adding Sub-Menu Links in Drupal
Once the Content Menu and Self-Service Menu are created in the Drupal site, content creators can easily add sub-menu links through the content creation or edit page. Here are the steps:

Steps to Add Sub-Menu Links:
Log in to the Drupal Admin Interface:

Ensure you have the appropriate permissions to add or edit content and manage menu links.
Navigate to Create or Edit Content:

Go to the desired content creation page (e.g., "Add Content" under "Content" in the admin toolbar).
Alternatively, if you’re editing existing content, locate the content via the "Content" tab and click on "Edit" for that specific item.
Locate the Menu Settings Option:

On the content creation or edit page, scroll down to find the "Menu Settings" option, typically located towards the bottom of the page.
Click to expand the "Menu Settings" section.
Enable Menu Link Creation:

Check the box labeled "Provide a menu link." This action will allow you to add a link to either the Content Menu or the Self-Service Menu.
Configure the Menu Link:

Menu Link Title: Enter the title you want to appear in the menu.
Parent Item: From the dropdown list, select the appropriate parent menu where you want this link to appear:
Choose "Content Menu" for links related to content navigation.
Choose "Self-Service Menu" for links related to user self-service pages.
Weight: Optionally, set the "Weight" of the menu item to determine its order relative to other menu items. Lower numbers appear higher in the list.
Save and Publish:

Once you’ve configured the menu link, save the content as usual.
Upon saving, the new sub-menu link will be added under the selected parent menu, making it accessible through the site’s navigation.
Additional Notes:
You can always return to edit the content and adjust the menu settings if needed.
The changes will reflect immediately in the site's navigation menus after saving the content.





Default Error Handling in Drupal for Menu Management
Form Validation:

Description: When creating or editing a menu link, Drupal automatically validates the input fields. If required fields (like the "Menu link title" or "Link path") are left blank, or if an invalid URL is entered, Drupal will display an error message and prevent the form from being submitted until the errors are resolved.
User Feedback: Users are alerted with a red error message near the problematic field, explaining what needs to be corrected.
Permission Checks:

Description: Drupal checks the user’s permissions before allowing access to menu management functions. If a user without the necessary permissions tries to create, edit, or delete a menu link, Drupal will deny access and display an "Access Denied" message.
User Feedback: The user sees an "Access Denied" message or is redirected to a page explaining they do not have the necessary permissions.
Path Validation:

Description: Drupal checks whether the path entered in the "Link path" field is valid. If the path points to a non-existent or unpublished page, Drupal will flag this and may display an error message.
User Feedback: A warning or error message is displayed if the entered path does not match any existing content or valid URL.
Conflict Resolution:

Description: Drupal handles potential conflicts in menu structure, such as duplicate paths or titles, by appending numeric suffixes or issuing warnings. This helps prevent conflicts that could cause navigation issues.
User Feedback: Drupal may automatically adjust conflicting items or provide a notification to the user about the conflict.
Automatic Menu Item Removal:

Description: If a piece of content is deleted, any associated menu links pointing to that content are automatically removed. This prevents broken links from appearing in the menu.
User Feedback: No direct feedback is usually provided, but the menu item will no longer appear after the content is deleted.
Error Logging:

Description: Drupal logs various errors, including issues related to menu management, in the system logs. These logs can be accessed by administrators to diagnose and resolve issues.
User Feedback: Administrators can view detailed error messages and logs under "Reports" > "Recent log messages" to troubleshoot issues.
Cache Management:

Description: Drupal automatically clears relevant cache entries when menu structures are updated. This ensures that changes are reflected across the site, minimizing issues caused by stale cache data.
User Feedback: While this process is automatic, users can manually clear the cache if they notice that changes are not being immediately reflected.
Handling Missing Parent Items:

Description: If a menu link is assigned a parent item that is later removed, Drupal will reassign the orphaned menu link to the top level of the menu or another valid parent. This prevents the link from being lost.
User Feedback: The link remains visible in the menu, but its position may change.
