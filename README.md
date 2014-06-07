dbtohtml
========

This script connects to a running database, inspects the tables, and generates an
HTML file that can be used to conveniently browse the structure of the tables.

#### Usage
```bash
groovy DbToHtml.groovy /path/to/configFile
```

The configFile is a java properties file containing the database connection details,
path to output file, and title for the HTML page.  For example:

#### Sample configFile
```
db_url = "jdbc:mysql://localhost/dbname"
db_username = "username"
db_password = "password"
output_file = "/path/to/data-model.html"
title = "My Data Model"
favicon = "https://example.com/favicon.ico"
```

If the db_password is not provided in config, you will be prompted for the password.
