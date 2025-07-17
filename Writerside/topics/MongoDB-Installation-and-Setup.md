# MongoDB Installation and Setup (Windows)

## Pre-Installation

MongoDB community edition supports the following 64-bit versions of windows on x86_64 architecture:

- Windows Server 2022
- Windows Server 2019
- Windows 11

## MongoDB Installation Steps

### Step 1: Download MongoDB

MongoDB is available in two server editions: Community and Enterprise. The community version is free and suitable for learning. To install MongoDB Community Edition, use the MongoDB Installer wizard.

The installation process installs both the MongoDB binaries as well as the default configuration file **<install directory>\bin\mongod.cfg.**

### Step 2: Download the installer

- Download the MongoDB Community .msi installer from the following link: [MongoDB Download Center](http://mongodb.com/try/download/community?tck=docs_server)
- In the Version dropdown, select the version of MongoDB to download.
- In the Platform dropdown, select Windows.
- In the Package dropdown, select msi. And, finally
Click Download.

### Step 3: Run the MongoDB installer

- For example, from the Windows Explorer/File Explorer: Go to the directory where you downloaded the MongoDB installer (.msi file). By default, this is your Downloads directory.
- Double-click the .msi file.

### Step 4: Follow the MongoDB Community Edition installation wizard.

#### Choosing the Setup type

You can choose either the complete(recommended for most users) or Custom setup type. The Complete setup option installs MongoDB and the MongoDB tools to the default location. The Custom setup option allows you to specify which executables are installed and where.

#### Service Configuration

Starting in MongoDB 4.0, you can set up MongoDB as a Windows service during the installation or just install the binaries.

## Command-line Shell (Mongosh) Installation

After MongoDB installation, install Mongosh. This is a command-line shell and interactive JavaScript interface for MongoDB, that provides easy ways to interact with MongoDB databases and perform various operations and queries.

**Note: The MongoDB Shell (mongosh) is not installed with MongoDB Server. You need to follow the mongosh installation instructions to download and install mongosh separately.**

### Mongosh Installation steps:

- Open the MongoDB Download Center.
- In the Platform dropdown, select Windows 64-bit (8.1+) (MSI)
- Click Download.
- Double-click the installer file
- Follow the prompts to install mongosh.

On Windows, mongosh preferences and configuration options are stored in this directory: **%APPDATA%/mongodb/mongosh**