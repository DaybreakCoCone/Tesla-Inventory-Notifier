<img width="1890" height="790" alt="b10dc8cb-0b49-4b41-9a6f-41f1b29aaa14" src="https://github.com/user-attachments/assets/0cfeb1bd-02ed-43e9-912b-8a7043458e7d" />
 ## Tesla Inventory Userscript

A Tampermonkey userscript that automatically reads Tesla inventory cards, extracts exterior color, interior color, wheel size, and drive type (AWD/RWD), and pushes notifications to your phone via Pushover.
It supports a collapsible control panel, random auto‑refresh, one‑click copy of a fixed referral link, and saving your Pushover credentials. Notifications are sent only when cars are detected.

---

## 1) Install the Userscript

1. Install a userscript manager in your browser, such as:
   - [Tampermonkey](https://www.tampermonkey.net/) (Chrome, Edge, Safari) **recommended**
   - [Violentmonkey](https://violentmonkey.github.io/) (Chrome, Firefox)

2. After installing a userscript manager, click the link below to install the script:

   **[Click here to install the latest script]([https://raw.githubusercontent.com/DaybreakCoCone/Tesla-inventory-userscript-CN-/main/tesla-inventory-reporter.user.js)](https://greasyfork.org/en/scripts/550091-tesla-inventory-notifier-v5-0)**

3. Once installed, you should see “Tesla Inventory Reporter” enabled in your userscript manager icon at the top‑right of the browser.

---

## 2) Configure Pushover (Get User Key & API Token/Key)

Pushover is a service that delivers messages to your phone, tablet, or desktop.
To enable the script to send you inventory notifications, complete the steps below.

### 2.1 Sign up & log in
- Go to https://pushover.net/ → click **Sign Up** to register and log in.
- After logging in, find your **User Key** at the top of the Dashboard and copy it for later.

### 2.2 Install the app & register your device
- Install Pushover on your phone:
  - iOS: App Store → search “Pushover”
  - Android: Google Play → search “Pushover”
- Open the app, log in, and allow notification permissions.
- Confirm your device appears as **Registered** under “Your Devices” on the Dashboard.

### 2.3 Create an application (get API Token/Key)
- On the Dashboard, open **Your Applications** → **Create an Application/API Token**.
- Choose a name (e.g., “Tesla Inventory Reporter”). After creation, copy the **API Token/Key**.

### 2.4 Fill in your credentials in the script panel
- Open the Tesla inventory page:  
  **https://www.tesla.com/inventory/new/my?referral=xuan634381&redirect=no&range=200&PaymentType=lease**
- In the bottom‑right panel, fill in:
  - **Pushover User**: your **User Key**
  - **Pushover Token**: your **API Token/Key**
- Click **Save Push Configuration**.
- Pick a model that’s in stock and click **Report Now** to verify that your phone receives a notification.

---

## 3) Usage

Open the Tesla inventory page:  
**https://www.tesla.com/inventory/new/my?referral=xuan634381&redirect=no&range=200&PaymentType=lease**

From the bottom‑right panel you can:

- **Report Interval** — number of seconds between page parses.
- **Auto Refresh** — when enabled, the script refreshes the page at random intervals.
- **Refresh Range (seconds)** — set the minimum/maximum random refresh seconds.
- **Report Now** — manually parse the page and send a notification immediately.
- **Pause / Run** — pause/resume the script anytime.
- **Copy Referral** — one‑click copy of the referral link above.

**Note:** If this userscript helps you, consider using my referral link when ordering to receive an extra three months of FSD (approx. USD $297 value).

---

## Example notification messages

1. **[AWD]** Exterior: White / Interior: Black / Wheels: 19  
2. **[RWD]** Exterior: Red / Interior: White / Wheels: 20

---

## Troubleshooting

- **The panel doesn’t appear**: Ensure the userscript is enabled for `tesla.com` pages in your userscript manager.
- **No notifications**: Verify your Pushover **User Key** and **API Token/Key**, and that your device is registered and allows notifications.
- **Auto‑refresh not working**: Confirm that **Auto Refresh** is enabled and that the **Refresh Range** has reasonable values (e.g., 20–60 seconds).
- **Duplicate or missing card info**: Reload the page; if it persists, file an issue with screenshots and browser console logs.

---

## Privacy & Data

- Your Pushover credentials are stored locally by the userscript manager and are used only to send notifications you’ve requested.
- This project does not collect personal data or send it to third‑party servers (other than Pushover, which you explicitly configure).

---

## Disclaimer

This project is an independent, community‑driven userscript and is **not** affiliated with, endorsed by, or sponsored by Tesla, Inc.
“Tesla” and related marks are trademarks of their respective owners. Use this script at your own risk and in accordance with Tesla’s website terms.
Do not use the script to spam or overload Tesla services. You are responsible for complying with local laws and site policies.

---

## Changelog

See **[CHANGELOG.md](./CHANGELOG.md)**.

---

## License

This project is distributed under the **MIT License**. See **[LICENSE](./LICENSE)** for details.
