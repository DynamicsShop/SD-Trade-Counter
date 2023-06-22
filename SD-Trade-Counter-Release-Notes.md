## SD Trade Counter Releases

### 3.2.1

#### Enhancements

- AppSource App - A change was made to limit the SD ISV Tenant Subscriptions page to display just our SD ISV AppSource Apps and not other SD PTE Apps.

#### Bug Fixes

- AppSource App - When selecting SD Trade Counter activity pages in the Tell Me/Search in a BCv22 environment, the activity pages were hanging.

### 3.2.0

#### Enhancements

- AppSource App - An option was added to the SD Trade Counter Setup,  Prompt Delete On Sales Order Exit, to allow users to leave an SD Trade Counter Order without being prompted to save or discard changes. A subscriber was also added to allow for custom functionality when a user navigates out of an SD Trade Counter Order. 

- AppSource App - Standard document release functionality was added to Trade Counter Sales Orders. Users can choose the Show Advanced Order Actions option in the Locations Setup. If this option is enabled, users can see the Release and Reopen actions in the SD Trade Counter Sales Order. An event subscriber was surfaced for before release and after release.

- AppSource App - Code was refactored to handle future removal of item cross reference. 

- AppSource App - There is no option to print a despatch docket or a sales invoice if a user chooses to pay for an order by choosing Sale on Account. An event subscriber was created to allow codeunit 81 or 82 to be called when Sales on Account is chosen. 

- AppSource App - A subscriber was added to allow a variation to the default selection of "1 - Cash" in the "Please Select Customer Type" prompt that is displayed when users choose to create a new Trade Counter Order, Refund or Quote. The subscriber also allows the text in the Please Select Customer Type prompt to be modified.  

- AppSource App - A subscriber was created to allow the selection of the customer account from the customer list to be overwritten. 

- AppSource App - A change was made to allow for an SD Trade Counter User to have a blank salesperson code in the SD Trade Counter User Setup.

- AppSource App - A change was made to allow for an SD Trade Counter User to have a blank location in the SD Trade Counter User Setup.

- AppSource App - SD Trade Counter Users with no location specified in the SD Trade Counter Users Setup, can view transactions from all Locations in the SD Trade Counter Role Centre KPIs.

- AppSource App - Indirect permission was granted to delete the Sales Header on Posting Orders.

- AppSource App - A change was made on Posting to set the Posting Date to the Work Date.

- AppSource App - A subscriber was added to the delete action for the Sales Line.

#### Bug Fixes

- AppSource App - A change was made to the ISV Licence Notification procedure in SD Trade Counter to fix an issue that would raise an error when the language is changed from English to another language. 

### 3.1.0

#### Enhancements

- BCv21 App - The Licence Message displayed on first install of SD Trade Counter was changed to prompt the user to activate a free trial and to choose Assisted Setup from the Setup Card to create demo data. 

- BCv21 App - A page was created to display all the Simply Dynamics Apps and subscription details for the tenant. 

- BCv21 App - The Licence Expiry message/notification was updated to display the App Name. 

- BCv21 App - The Product Activation Page was updated to point to the new CRM URL. 

- BCv21 App - The ToolTips were updated to look at our new website. 

- BCv21 App - Minor text changes were made to some pages on the Assisted Setup Wizard.

#### Bug Fixes

- BCv21 App - A fix was made to the code for licence key checks on the SD Trade Counter Role Centre.  

### 3.0.0

#### Enhancements

- BCv20 App - A change was made to allow more than one user at a time to log into the same till. 

- BCv20 App - A change was made to allow users to recall Quotes, Orders and Credit Memos even if they are not SD Trade Counter transactions. This transactions can be recalled using the Import action cue on the SD Trade Counter Transaction pages. 

- BCv20 App - The Ship-To-Address details on the Ship-to Address cue were rearranged. 

- BCv20 App - The External Document No. and the Your Reference fields were surfaced on the SD Trade Counter transaction pages. 

- BCv20 App - The Shipping Agent field was surfaced on the Ship-to Address cue on the SD Trade Counter transaction pages. 

- BCv20 App - A Boolean field was added to the Till Users Setup to Prompt for the Salesperson on every SD Trade Counter Transaction. This is to allow for when multiple users log in to the same till and users can choose their Salesperson Code. 

### 2.0.0

#### Enhancements

- BCv19 App - The SD Trade Counter Till Receipt was converted from C/AL to AL extensions. 

- BCv19 App - A User Role Centre was created for SD Trade Counter. 

- BCv19 App - The product was streamlined for fast cash out. 

- BCv19 App - A Till concept was added to SD Trade Counter. 

- BCv19 App - The SD Trade Counter objects were renamed to our ISV standards. 

- BCv19 App - C/AL objects were converted to AL extensions. 

- BCv19 App - A big button FactBox panel was added to the Sales Order page for touch screen use. 

- BCv19 App - SD Trade Counter logic and functionality was reworked to allow for optimised order entry. 

- BCv19 App - The Cash Out Screen was optimised for fast cash out. Various icons and actions were added to the Cash Out Screen. 

- BCv19 App - Standard notes and link actions were removed from the SD Trade Counter pages to keep pages as clear and as uncluttered as possible.   

- BCv19 App - The product was made usable for a touch screen environment. 

- Bcv19 App - Assisted Wizard Setup was added to the product. 

- BCv19 App - Permission Sets were created for the Product. 

- BCv19 App - If user Cashes Out using Multi Tender then all goes against the same Payment Method Code on Cash Out. 

- BCv19 App - In the Cash Out page a message is raised if the customer is paying cash and the user chooses Quick Pay Card. The message prompts to ask the user if they want to pay the balance by card. 

- BCv19 App - To enable users easily identify stock levels, the standard Sales Order Lines FactBox was added to the SD Trade Counter Order Entry page. 

- BCv19 App - When the Salesperson Code is validated into the Sales Order, the Trade Counter Location is now validated into the Sales Order Header and Lines. 

- BCv19 App - When choosing the New Account Order cue from the SD Trade Counter Role Centre, a list of Customers is now shown, the user selects the Customer, and a new order is created and populated with the chosen Customer. 

- BCv19 App - Functionality was developed to allow users sign into the SD Trade Counter Product.

- BCv19 App - When the user signs out during order entry and there are no details entered then the empty order is deleted. If the user signs out and there are details entered then prompt the user to save or discard the order.  

- BCv19 App - Made a change to ensure that on a new Sales Order all totals and fields are reset. 

- BCv19 App - The Quick Pay Cheque and the Quick Pay Voucher actions were removed from the Cash Out screen. 

- BCv19 App - The SD Trade Counter Setup Action was removed from the User Role Centre. 

- BCv19 App - Buttons with 5, 10, 20, 50 were added to the Cash Out screen to allow for quick input of cash amounts. 

- BCv19 App - To allow for ease of user input, the Take Payment action was added to the right of the Sales Order page. 

- BCv19 App - The default Salesperson Code associated with the logged in user defaults into the SD Trade Counter Order, Quote and Refund. 

- BCv19 App - The Barcode Scan field was repositioned above the General FastTab for ease of use and visibility. 

- BCv19 App - Allow for Salesperson filtering on the cues in the User Role Centre. 

- BCv19 App - The Remaining Amount on the Cash Out screen was made uneditable. 

- BCv19 App - Code was written to post to the payment journal on invoice of the order from the SD Trade Counter Payment Screen and apply the payment to the Invoice. A Payment Tracking table was created to record details of the individual Tender Lines that make up the overall payment. 

- BCv19 App - The Previous Line and the Next Line actions were removed from the Sales Order Entry page. 

- BCv19 App - Made a change to the barcode scanning so when an item is scanned the barcode in the Barcode Scan is blanked and the focus is put back into the Barcode Scan field. 

- BCv19 App - When the SD Trade Counter Sales Order page is open the focus is on the Scan Barcode field. 

- BCv19 App - Change the User Role Centres to filter by the currently logged in user by default. 

- BCv19 App - The Latest Version and AppSource URL fields were added to the About Page. 

- BCv19 App - The code was reviewed to ensure that the Licence Expiry Date prompts with 5 days to go is not stopping the SD Trade Counter functionality. 

- BCv19 App - The Allow HTTPClient Request is enabled on install of the product. 

- BCv19 App - Captions on objects were updated for future translations. 

- BCv19 App - The SD Trade Counter Role Centre Activities were created on separate pages to allow users to search on the individual SD Trade Counter Role Centre Activities in the Tell Me. 

- BCv19 App - The SD Trade Counter product was readied for AppSource Submission. 

- BCv19 App - Usage Categories were added to SD Trade Counter pages for Tell Me searchability.  

- BCv19 App - The Product Activation, Assisted Setup and About actions were added to the SD Trade Counter Setup Card as per our other Dynamics 365 Business Central Apps. 

- BCv19 App - The size of the code, description and name fields in SD Trade Counter were increased as per standard D365 BC changes. 

- BCv19 App - The ISV About page was added to the product. 

- BCv19 App - The objects were renumbered to the ISV range. 

- BCv19 App - Created a Z Report for the product. This report shows grand totals of the transactions at end of day. 

- BCv19 App - Rework the Barcode functionality in the product to ensure easy barcode scanning. 

- BCv19 App - The ISV Licence Controller was added to the product. 

- BCv19 App - Created an X Report for the product. This report shows detailed transaction history during the day. 

- BCv19 App - The product was rebranded to SD Trade Counter. 

- BCv19 App - An SD Trade Counter Manager Role Centre was created. 

- BCv19 App - The caption of the Daily Total option on the SD Trade Counter Your Managed Tills was changed to Display Daily Total.

- BCv19 App - The X Report Summary was renamed to X Report Daily Summary.

- BCv19 App - The Ship-to-Details action in the General FastTab of the SD Trade Counter Sales Order, Quote and Refund was removed as it is also surfaced as a button in the Options FactBox.

- BCv19 App - The SD Trade Counter Refund Receipt was showing the correct VAT description and amount on the lines but was showing an incorrect VAT Description at the end of the Report. This was reworked. 

- BCv19 App - The SD Trade Counter Sales Receipt was showing the correct VAT description and amount on the lines but was showing an incorrect VAT Description at the end of the Report. This was reworked.

- BCv19 App - In the SD Trade Counter Order or Refund pages if there is no email address in the email field and the Email Receipt is turned on prompt the user on selection of the Pay Now button.

- BCv19 App - The code to calculate the calculations on the SD Trade Counter Mangers Till KPI was reviewed.

- BCv19 App - Various user interface changes were made to the SD Trade Counter Order, Quote and Refund pages.

- BCv19 App - A  caption on the Z report was changed from Estimated Amount to Calculated Amount to reflect the value of the field.

- BCv19 App - The Z report was modified to have an option to run a test reconciliation.

- BCv19 App - The Location Code on the SD Trade Counter Order, Quote and Refund pages was set to not editable.

- BCv19 App - The prompt for initial licence activation of SD Trade Counter was moved to the SD Trade Counter Setup Card.

- BCv19 App - In the SD Trade Counter Setup Card the Setups FastTab Caption was changed to Locations.

- BCv19 App -  The captions of the various SD Trade Counter Setup Pages were updated.

- BCv19 App - The Till Login table and associated functionality was expanded to display the currently logged in user and to prevent more than one user logging into the same till.

- BCv19 App - A Till Login History table was created to store the details of the user and date and time of till login and logout.

- BCv19 App - When the Z report is run and the transactions on the till are reconciled, the users are now logged out the tills.

- BCv19 App - A new report similar to the layout of the SD Trade Counter X and Z reports was created with an additional section to show details of the transactions that went through the SD Trade Counter Cash Payment Screen.

- BCv19 App - The logic of the code was reworked so that the errors raised on posting the Sales Order are no longer displayed after the prompt to create a new Order in SD Trade Counter.

- BCv19 App - A Test Codeunit for AppSource submission was created. 

- BCv19 App - When initiating a till by running the SD Trade Counter Set Float processing report, the decimal places formatting were set.

- BCv19 App - Changes were made to make the various SD Trade Counter Setup pages editable on drill through of the KPI cues in the KPIs FastTab on the SD Trade Counter Setup Card.

- BCv19 App - The standard new, edit list, delete actions were added to a number of the SD Trade Counter Setup pages.

- BCv19 App - The message displayed in the SD Trade Counter Cash Payment screen when users pay by choosing the Quick Pay Card was updated. 

- BCv19 App - The message displayed in the SD Trade Counter Cash Payment screen when users try to Cash Out with less than the total owed was updated.

- BCv19 App - A boolean field was added to the SD Trade Counter Refund and Order pages to allow users control, per document, whether to email the receipt to the customer or not.

- BCv19 App - The placeholder fields in the SD Trade Counter Email Receipt Templates were updated to look at the Posted Sales Invoice or Posted Sales Credit Memo Headers.

- BCv19 App - Digital Signatures can be captured in the SD Trade Counter Orders, Refunds and Quotes on the Sales Header level and on post of these documents are transferred to the posted table.

- BCv19 App - Changes were made to captions on the SD Trade Counter Setup List for ease of user input and understanding.

- BCv19 App - KPI functionality was created to allow Managers to setup and close out their tills in SD Trade Counter.

- BCv19 App - The Document Default Line on the Sales and Receivables Setup is used to auto default in the line type on the SD Trade Counter Orders, Refunds and Credit Memos as per standard Microsoft Dynamics 365 Business Central.

- BCv19 App - Logic was created to allow for occurrences where error messages raised in the SD Trade Counter Payment Screen do not prevent the Payment Tracking Entry record from being created.

- BCv19 App - The float is now recorded as an opening balance transaction on the SD Trade Counter Payment Tracking table.

- BCv19 App - Journal Batches for Customer Payments can now also be defined at Till Level so separate Bank Accounts can be defined for Customer Payments at Till Level.

- BCv19 App - Functionality was added to SD Trade Counter to allow for users to log SKIMS taken from the Till.

- BCv19 App - In the SD Trade Counter Payment Screen, when choosing to Pay and Print Receipt with not enough tendered users are prompted with the remaining amount.  This logic was added to the Pay and Print Invoice button.

- BCv19 App - If no Card Types have been set up in SD Trade Counter then users should not be prompted with a blank screen when choosing to pay by card but given a message prompt.

- BCv19 App - The Location Code was made a mandatory field in the SD Trade Counter User Setup Table.

- BCv19 App - The extension on the standard User Setup was removed from the SD Trade Counter product as we now have our own Trade Counter User Setup. 

- BCv19 App - The prompts to the user to validate their SD Trade Counter licence were updated to reflect that of our other ISV products.

- BCv19 App - Functionality was added to SD Trade Counter to allow users close out the tills at the end of the day and reconcile the tills.

- BCv19 App - When paying by Card in the SD Trade Counter Payment Screen, users are now given the option to specify the Card Type.

- BCv19 App - A Cheque Amount button was added to the SD Trade Counter Payment Screen.

- BCv19 App - Functionality was added to the product to allow users easily add and update Ship-to Addresses for SD Trade Counter Orders, Refunds and Quotes.

- BCv19 App - Various User Interface changes were made to the SD Trade Counter Order, Quote and Refund Pages. A boolean was added to the SD Trade Counter User Setup to show or hide FaxtBoxes on the pages. Buttons were recaptioned.

- BCv19 App - The Actions from the Menu in the SD Trade Counter Order, Quote and Refund pages were removed and placed in the Options FactBox as buttons for ease of input.

- BCv19 App - Changes were made to the List page that is displayed when choosing the Recall buttons from within an SD Trade Counter Order, Quote or Refund.

- BCv19 App - The Cues on the SD Trade Counter Role Centre were filtered to Tills and Locations.

- BCv19 App - Functionality was added and actions surfaced to allow users easily email the various SD Trade Counter Documents Order, Quote and Refund, Sales Receipt and Refund Receipt. Email templates were added that users can use for emailing the Sale Receipt and the Refund Receipt.

- BCv19 App - Functionality was added to allow users to capture digital signatures on the SD Trade Counter Orders, Quotes and Refund pages.

- BCv19 App - Changes were made to the KPIs FastTab in the SD Trade Counter Setup Card.

- BCv19 App - In the SD Trade Counter Payment Screen, selecting Return on the Tendered Amount field brought users down to the Tender Lines. Users then had to scroll back up to select the Cash Amount or Card Amount buttons. The navigation in the page was updated for ease of user input.

- BCv19 App - The Links in the About Page were updated to point to our new website.

- BCv19 App - On the SD Trade Counter Payment Screen, the Pay and Print Receipt and the Pay and Print Invoice actions were moved from the menu onto the actual page as buttons.

- BCv19 App - Added validation to allow Trade Counter Quotes use the No Series as specified in the SD Trade Counter Setup. 

- BCv19 App - Changes were made to the User Role Centre. 

- BCv9 App - The SD Trade Counter Refund Receipt was converted from C/AL to AL extensions. 

- BCv19 App - When a Barcode is scanned into the Sales Order the Barcode field is set to blank.

- BCv19 App - Users cannot Cash Out with less than the total owed. 

- BCv19 App - For situations where a Credit Memo Refund for an Account Customer is given from the cash drawer a  Cash Receipt of type Refund is created and applied to the Credit Memo on the CLE. The Doc Type is Refund, the value posted is positive and the Doc. No. is set to the Credit Memo. If a Credit Memo Refund on SD Trade Counter is applied to the Account (not put through Cash Drawer) then no Cash Receipt of Refund is created and the Credit Memo is kept open on the CLE. 

- BCv19 App - The Latest ISV Licence Control with the fix to Free Trials in Public Environment was added to the Product. 

- BCv19 App - Changes were made to taking payments for Account Customers. The Customer Balance is displayed on the Cash Out page and an option is available to apply the change form the sale to the Account balance. 

- BCv19 App - For ease of use in Recall Document Lists the Amount and Remaining Amount were added to the list so users can differentiate between the orders. 

- BCv19 App - Create a Change Till action and functionality on the SD Trade Counter TIll Login page.

- BCv19 App - The Trade Counter Setup Action on the Role Centre was recaptioned to Setup. 

- BCv19 App - In the SD Trade Counter Setup show the Report Name when displaying the drop downs on the Report Fields. 

- BCv19 App - The structure of the SD Trade Counter setup card was changed. General and KPI fasttabs and a list part page were added.  

- BCv19 App - ISV Licence Controller checks were added to the code. 

- BCv19 App - The SD Trade Counter Role Centre was removed from the Trade Counter pages displayed in the Tell Me. 

#### Bug Fixes

- BCv19 App - Postings for Account Customers with a Refund given from the Till should have a Type Refund with a positive entry posted and allocated to the Credit Memo.

- BCv19 App - If the Email Receipt option was switched off in the SD Trade Counter Order or Refund but a new line was added,  the Ship to Address added or updated, or a Signature Added then the Email Receipt option was switched on again.

- BCv19 App - Choosing the Ship-to Address button in the SD Trade Counter Orders, Quotes or Refunds was not displaying the correct Ship-to Address details for the record.

- BCv19 App - Choosing Email Receipt was not sending the Emails when Pay&Print was selected in the is not sending the email in the SD Trade Counter Payment Screen.

- BCv19 App - When Background Scanning was turned on then when an item was scanned the Type field on the Sales Line was blanked out. 

- BCv19 App - When the Z report was run the reconciled checkbox on the reconciled line was not updated.

- BCv19 App - Fixed an issue where filter warnings were raised on the SD Trade Counter Order page when a Recalled Order for an Account Customer was posted. 

- BCv19 App - A fix was made to prevent users from overpaying a Credit Refund to a customer. 

- BCv19 App - An error that there was no  Cust. Ledger Entry within the Filter when choosing to Pay&Print Invoice was preventing record insertion into the SD Trade Counter Payment Tracking table. This was caused by the fact that a journal line couldn't be posted and was fixed by applying the payment line to invoice only if the invoice is "Open". 

- BCv19 App - The Refunds in SD Trade Counter were not working correctly. 

- BCv19 App - The Recall functions in the SD Trade Counter Order pages were not working. 

- BCv19 App - The Take Payment action was added to the Cash Sale Order for the Account Sales Order screen. 

- BCv19 App - In the Take Payment screen the change field was not updating when cash lines were deleted. 

- BCv19 App - Receipts and Invoices were not printing after posting in the Take Payment screen. 

- BCv19 App - The Unit Price was not editable on the sales order lines. 

- BCv19 App - The new Account Sale was not initialised and displayed on the screen when in a Cash Sales Order and the Account Sale action was selected. 

- BCv19 App - Fixed an issue where blank Cash Sales Orders were being created in the background when the Cash Sale action in the SD Trade Counter Sales Order was selected. 

- BCv19 App - A payment entry was not being created after taking payment in SD Trade Counter. 

- BCv19 App - Changed functionality to allow a user to easily pause order entry and move on to a new order. 

- BCv19 App - The Till Invoice ID defined in the SD Trade Counter Setup was not printing when a payment was made. 

- BCv19 App - An error was raised when a Till Code was inserted into the SD Trade Counter Till Setup. 

- BCv19 App - When adding a Salesperson Code to the Trade Counter User Setup the Salesperson Name was not shown until you exited and then reopened the page. 

- BCv19 App - The version of the released App was showing an incorrect version. 

- BCv19 App - The Totals were not being calculated correctly in the Cash Out screen. 

- BCv19 App - An issue with the Reset button on the Cash Out page was fixed. 

### 1.0.0

#### Enhancements

- Initial C/AL Build of SD Trade Counter. 
