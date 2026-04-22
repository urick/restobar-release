# RestoBar+ Downloads

RestoBar+ is a professional restaurant and bar POS system developed by [IVA Elektronik](https://www.ivaelektronik.com/).

## Download

Download the latest installer from the [Releases](https://github.com/urick/restobar-release/releases/latest) page.

## System Requirements

- **OS:** Windows 10 or Windows 11 (64-bit)
- **RAM:** 4 GB minimum
- **.NET Framework:** 4.7.2 or later (installer will install 4.8 if needed)
- **SQL Server:** Any edition (Express, Standard, Enterprise). The installer can install SQL Server Express automatically.
- **Disk Space:** ~200 MB for the application + database storage

## Installation

1. Download `RestoBar+_Setup.exe` from the latest release
2. Run the installer as Administrator
3. Choose installation type:
   - **Server** — Installs SQL Server, creates the database, and sets up the API service
   - **Client** — Installs only the POS application (connects to an existing server)
   - **Custom** — Choose individual components
4. Configure the database connection on the Database Configuration page:
   - **SQL Server Instance** — auto-detected if SQL Server is already installed
   - **Database Name** — default: `resto`
   - **SQL Username** — default: `sa`
   - **SQL Password** — the password set during SQL Server installation
5. Complete the installation

## Components

| Component | Description |
|-----------|-------------|
| **RestoBar+ POS** | Main point-of-sale application (always installed) |
| **SQL Server Express** | Database engine (optional — skip if already installed) |
| **Database Init** | Creates and initializes the database schema |
| **RestoSync API** | Background service for the Android waiter app |
| **POSAdmin** | Back-office administration tool |
| **FiskalizeThis** | Fiscal device integration service |
| **SSMS** | SQL Server Management Studio (optional) |

## Updating

RestoBar+ includes auto-update functionality. When a new version is available, the application will notify you on startup.

For manual updates, download the latest installer and run it — existing data and settings are preserved.

## Uninstalling

Use Windows **Settings > Apps > RestoBar+** or run the uninstaller from the Start Menu. The uninstaller will:
- Stop and remove the RestoSync API service
- Remove application files
- **Note:** The database is NOT removed during uninstall to protect your data

## Support

- **Phone:** 042 220 356
- **Website:** [ivaelektronik.com](https://www.ivaelektronik.com/)

---

*Built and published automatically by IVA Elektronik*
