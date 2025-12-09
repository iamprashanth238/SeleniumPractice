# 🧪 Selenium Automation Practice Site (SPA)

A lightweight, single-page application (SPA) built with HTML, CSS, and Vanilla JavaScript designed specifically for practicing **Selenium WebDriver**, **Playwright**, **Cypress**, or **Puppeteer** automation scripts.

No backend server, database, or installation is required. Just open the file and start coding your tests!

## 🚀 Features for Automation Practice

This application includes various HTML elements and logic to simulate real-world test scenarios:

* **Authentication Flow**: Login and Registration forms with validation.
* **Data Persistence**: Uses Browser `localStorage` to save registered users (simulating a real database). New registrations persist across page refreshes.
* **Synchronization (Waits)**: A dedicated section to practice Explicit Waits (5-second loading delay).
* **Web Tables**: Dynamic tables to practice handling rows, columns, and finding specific data.
* **Alerts & Popups**: JavaScript Alerts, Confirm boxes, and Prompts.
* **Form Elements**: Text inputs, Radios, Checkboxes, Dropdowns (Select), and Date pickers.
* **Iframes**: Embedded content to practice switching context.
* **Mouse Actions**: Areas specifically designed for Hover and Double Click events.

## 🛠️ Quick Start

### Option 1: Run Locally
1.  Clone this repository:
    ```bash
    git clone [https://github.com/your-username/selenium-practice-site.git](https://github.com/your-username/selenium-practice-site.git)
    ```
2.  Navigate to the folder.
3.  Double-click **`index.html`** to open it in your browser.
4.  Copy the file path from the address bar (e.g., `file:///C:/Users/You/index.html`) to use in your Selenium script `driver.get()`.

### Option 2: GitHub Pages (Optional)
If you enable GitHub Pages for this repo, you can access it via a public URL like:
`https://your-username.github.io/selenium-practice-site/`

## 🔑 Default Credentials

The system comes pre-loaded with 10 fake users. You can use the administrator account or any user from the list.

| Username | Password | Role |
| :--- | :--- | :--- |
| **admin** | **admin123** | Admin |
| **john.doe** | **password123** | User |
| **alice.j** | **alicepass** | Editor |

> **Note:** You can see the full list of users in the browser Console (F12) or register your own.

## 🧪 Practice Scenarios

Here are some standard automation challenges you can try on this site:

### 1. End-to-End Registration Flow
1.  Navigate to the Login Page.
2.  Click "Register Here".
3.  Fill out the form with a unique username.
4.  Submit and verify the success message.
5.  **Challenge:** Login with the newly created credentials and verify the username appears on the Dashboard.

### 2. Handling Explicit Waits
1.  Login and go to the "Dynamic Waits" section.
2.  Click the "Start 5s Timer" button.
3.  **Challenge:** Use `WebDriverWait` (or `ExpectedConditions`) to wait until the text "Element Loaded Successfully" becomes visible before asserting success.

### 3. Web Table Iteration
1.  Login to the Dashboard.
2.  Locate the User Table.
3.  **Challenge:** Write a script that iterates through the table rows, finds the row containing "Alice Johnson", and retrieves her Role (Editor).

### 4. Alert Handling
1.  Go to the Alerts section.
2.  Click the "Confirm" button.
3.  **Challenge:** Switch to the Alert context, read the text, and accept (Click OK) or dismiss (Click Cancel) it.

## 🧹 Resetting Data

Since this app uses `localStorage`, your created users will remain saved in your browser.
To clear your custom data and revert to the original 10 users:
1.  Login to the dashboard.
2.  Click the **"Reset to Default Data"** button under the Web Table.

## 🤝 Contributing

Feel free to fork this repository and add more complex elements (like Shadow DOM, Drag and Drop, or File Uploads) to make the practice more challenging!

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
