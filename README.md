# ERPNext Test Environment (Codespaces)

This repository contains a 1-click GitHub Codespaces setup to test ERPNext with the following apps:
- **ERPNext v15**
- **India Compliance** (GST, e-Invoice, e-Way Bill, TDS/TCS)
- **HRMS**
- **Helpdesk**
- **Print Designer**

## How to use

1. Push this folder to a new GitHub repository.
2. Go to the GitHub repository page.
3. Click on **Code** -> **Codespaces** -> **Create codespace on main**.
4. The first launch will take 5–15 minutes as it builds the Docker image with all the custom apps.
5. Once the Codespace starts, wait a minute for the database and web server to initialize.
6. Open the **PORTS** tab in Codespaces and click the URL next to port `8080`.
7. You should see the ERPNext login screen!

### Credentials

- **Username**: `Administrator`
- **Password**: `admin`

*(If the password `admin` doesn't work, wait a moment or restart the `frontend` container, as the initialization scripts may still be running).*

## Modifying Apps

If you want to add or remove apps, edit the `apps.json` file in the root directory, then rebuild the Codespace container.
