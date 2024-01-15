# mysqli_extended

"mysqli_extended" is a PHP class that inherits from the standard mysqli class, introducing additional, easy-to-use methods tailored to simplify common tasks for PHP developers working with MySQL databases. This extension aims to enhance the usability of the original mysqli functionalities by providing a more intuitive and streamlined interface, empowering developers to write cleaner and more efficient database-related code.

### Usage:

```
require_once(path/mysqli_extended.php);

$conn = new mysqli_extended($hostname, $username, $password, $database);

$conn->execute("SELECT * FROM table WHERE id = ?", $id);
```

Native mysqli methods are still supported.

### Methods (current):

- **execute()** basic use for query executions. Uses prepared statements, 1 or more arguments can be provided.
- **fetchAll()** returns an array of multiple records
- **fetchAssoc()** returns an associative array of a record from database
- **lastInsertID()** equivalent to $conn->insert_id

###### Disclaimer:

This PHP Class is a replica of David Adams' Super-fast PHP MySQL Database Class
link: (https://codeshack.io/super-fast-php-mysql-database-class/)

Visit the link to get enlightened with full functionality of the `execute()` function (in his version is `query()`).

### TO-DO's

- add the basic CRUD functions
- future bugs fixes
