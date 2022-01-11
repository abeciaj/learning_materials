# Mac Setup
On macOS, you can install MySQL easily using [Homebrew.](https://brew.sh/) Run:
```
brew install mysql
```
You can now start the MySQL server by running:
```
brew services start mysql
mysql --version
```

# Ubuntu Setup
To install it, update the package index on your server if you’ve not done so recently, then install the mysql-server package:

```
sudo apt update
sudo apt install mysql-server
mysql --version
```

# Windows Setup
1. Download MySQL Installer [here](https://dev.mysql.com/downloads/installer/) and execute it.
2. Determine the setup type to use for the initial installation of MySQL products. For example:

   - **Developer Default**: Provides a setup type that includes the selected version of MySQL Server and other MySQL tools related to MySQL development, such as MySQL Workbench.

    - **Server Only**: Provides a setup for the selected version of MySQL Server without other products.

   - **Custom**: Enables you to select any version of MySQL Server and other MySQL products.

3. Install the server instance (and products) and then begin the server configuration by following the onscreen instructions. For more information about each individual step, see Section 2.3.3.3.1, [MySQL Server Configuration with MySQL Installer.](https://dev.mysql.com/doc/refman/8.0/en/mysql-installer-workflow.html#mysql-installer-workflow-server)