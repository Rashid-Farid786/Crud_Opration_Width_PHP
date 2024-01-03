# Crud_Opration_Width_PHP 
#### One file Perform Crud operation Easy 
#### in This File All Crud Operation Created Like 

#### select table one paramer is table name

    settable($table)	

#### return current table name no param requered 

    gettable()

#### Select All Data From Data Base return object no param 

    all()

#### Find and data With id and return object with data.passed id where data find in database 

    find($id) 

#### Insert data to database and return object width insert row id.the array keys database colums name and value where insert in database 

    insert(array())

#### Update data from database.the array keys are database fields names and the value where updated to.the second param is id where data update

    update(array(),$id)

#### delete data where row id passed in and return object width deleted row in 

    delete($id) 

## example : 

    require_once "connection.php"; 
    $con=new connection(host_name,user_name,password,database_name); 
    $con->settable(table_name); 
    $con->all();


#### Error handler is Created in this File if error accur then eroor handler Call Automatically
## Example :

    require_once "connection.php";
    $con=new connection("host","user","password","db_name");
    $con->settable("test");
    $con->all();

## output :

#### Table 'db_name.test' doesn't exist on line number 3

#### also html popup error oe success message javaScript function available the function name Is mesaage(message,error/success)
#### and the popup tag css available in it.

## example :

    <script>
    message("Error Found","error");
    </script>

#### this message tag Show top right corner in the web page
