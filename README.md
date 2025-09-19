Tesla Inventory Userscript

A Tampermonkey userscript to automatically read Tesla inventory cards, extract exterior color, interior color, wheel size, and drive type (AWD/RWD), and push notifications to your phone via Pushover.
Supports panel collapse, random auto-refresh, fixed referral code one-click copy, and saving your Pushover credentials. Notifications are only sent when cars are detected.

1. Install the Userscript

Install a userscript manager in your browser, such as:

Tampermonkey
 (Chrome, Edge, Safari) (recommended)

Violentmonkey
 (Chrome, Firefox)

After installing a userscript manager, click the link below to install the script:

Click here to install the latest script

Once installed, you should see “Tesla Inventory Reporter” enabled in the userscript manager icon at the top-right of your browser.

2. Configure Pushover (Get User Key and API Token/Key)

Pushover is a service that delivers messages to your phone, tablet, or desktop.
To enable the script to send inventory notifications to you, follow these steps:

2.1 Sign Up and Log In

Visit https://pushover.net/
 → click Sign Up to register and log in.

After logging in, you’ll see your User Key at the top of the Dashboard — copy and save it.

2.2 Install the App and Register Your Device

Install Pushover on your phone:
iOS: Search “Pushover” in the App Store
Android: Search “Pushover” on Google Play

Open the app, log in with your account, and allow notification permissions.

Confirm your device appears under “Your Devices” on the Dashboard as Registered.

2.3 Create an Application (Get API Token/Key)

On the Dashboard, go to “Your Applications” → “Create an Application/API Token.”

Choose a name (e.g. Tesla Inventory Reporter). After creation you’ll receive your API Token/Key.

Copy and save it.

2.4 Enter Your Credentials in the Script Panel

Open the Tesla inventory page (https://www.tesla.com/inventory/new/my?referral=xuan634381&redirect=no&range=200&PaymentType=lease
).

In the bottom-right panel of the page, fill in:

Pushover User: your User Key

Pushover Token: your API Token/Key

Click “Save Push Configuration.”

Pick a model that’s in stock and click “Report Now” to test if your phone receives the notification.

3. Using the Userscript

Open the Tesla inventory page (https://www.tesla.com/inventory/new/my?referral=xuan634381&redirect=no&range=200&PaymentType=lease
).

In the bottom-right panel you can:

Report Interval: Set how many seconds between parsing the page.

Auto Refresh: Enable to let the script refresh the page at random intervals.

Refresh Range (seconds): Configure the min/max random refresh interval.

Report Now: Manually parse the page and send a notification immediately.

Pause/Run: Pause the script anytime.

Fixed Referral One-click Copy: Click “Copy Referral Code” to copy (https://www.tesla.com/inventory/new/my?referral=xuan634381&redirect=no&range=200&PaymentType=lease
).

Note: If this plugin helps you, consider using my referral code when placing an order to receive an extra three months of FSD (worth $297).

Example Notification Content:

[AWD] Exterior: White / Interior: Black / Wheels: 19

[RWD] Exterior: Red / Interior: White / Wheels: 20

📝 Changelog (excerpt)

See CHANGELOG.md

License

This project is licensed under the MIT License
.