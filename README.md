# phpMyAdmin on Laragon (Fix Forbidden Issue)

## Introduction

If you encounter **phpMyAdmin Forbidden** or **403** errors when using Laragon, this is **normal behavior**.

⚠️ **Important Notice**  
Laragon **does NOT include phpMyAdmin by default** in their installer.  
Therefore, when you try to access phpMyAdmin without installing it manually, Laragon will show a *Forbidden* or *Not Found* error.

To fix this issue, you need to manually install phpMyAdmin by following the steps below.

---

## Requirements
- Laragon installed
- PHP enabled in Laragon
- Apache or Nginx running
- MySQL/MariaDB running
- Internet connection

---

## Installation Steps

1. Download the latest phpMyAdmin package.  
   The downloaded file name will look like: phpMyAdmin-5.2.3-all-languages.zip
2. Extract the zip file into the following directory: path/to/laragon/etc/apps
3. After extracting, **rename the extracted folder**:
From   : phpMyAdmin-5.2.3-all-languages
To     : phpMyAdmin


⚠️ **CRITICAL**  
The folder name **must be exactly `phpMyAdmin`**.  
If you do not rename it correctly, Laragon will not detect phpMyAdmin and the Forbidden error will persist.

4. Restart **Laragon**.

---

## Access phpMyAdmin

After restarting Laragon, you can access phpMyAdmin via:
- Open your browser and go to: http://localhost/phpmyadmin
---

## Troubleshooting

- Ensure Apache/Nginx and MySQL are running.
- Double-check the folder path: laragon/etc/apps/phpMyAdmin

- Make sure the folder name is **case-sensitive** and spelled correctly.

---

## Conclusion

The phpMyAdmin Forbidden issue in Laragon is **not a bug**, but a design choice.  
Manual installation is required to enable phpMyAdmin support.

Once installed correctly, phpMyAdmin will work normally without errors.



