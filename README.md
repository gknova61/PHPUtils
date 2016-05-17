# PHPUtils
My Personal Library for various conveniences in PHP.

### Method Documentation
  - `bit_to_bool($bit)` - Returns a boolean from a binary bit (int 0 or 1)
  - `bool_to_bit($bool)` - Returns a binary bit (int 0 or 1) from a boolean
#####The above methods are good for storing booleans in a MySQL database in a performance-friendly fashion
 
  - `closeScript($message = '')` - A version of die() that will also close the MySQL connection on $con. Must specify a message for the script to die
  - `cleanString($string)` - Returns a string with stripped out extra characters (everything but alphanumerics)
  - `generate_random_string($nbLetters)` - Returns a random string. $nbLetters is the length of the string
  - `get_client_ip()` - Returns a client's ip address in 0.0.0.0 form. False if not found. This method is to be improved for ipv6 and more clients
  - `get_random_string($valid_chars, $length)` - Returns a random string. $valid_chars is an array of characters that the string will be made up of. $length is the length of the string
  - `query($query)` - Run a MySQL query on $con connection variable (must be already set)
  - `MySQLConnect()` - Connect to MySQL based on $dbServer, $dbUsername, $dbPassword, $dbDatabse variables that must be already set. Returns the connection variable
 * Recommended: Set the output of this function to a variable $con if you plan on using the above query function i.e. $con = MySQLConnect();
  - `toFloat($string)` - Convert any string into a float, stripping out all extra characters
  
