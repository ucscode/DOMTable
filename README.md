# DOMTable
A PHP Library that uses DOMDocument &amp; Nodes to create custom HTML table

### Code Sample

```php

## ------ [ SHORT SUMMARY OF HOW TO USE DOMTable ] ------

// create table instance;

$table = new DOMTable( 'tablename' );


// set table column;

$table->columns( array(
	"id",
	"name" => "Full Name"
) );


// set table data;

$table->data( array(
	array( "id" => 1, "name" => "My name" ),
	array( "id" => 1, "name" => "Your name" ),
) );


// set table limit;

$table->chunk(5); // set max number of rows per page;

$table->page(1); // define the current page;


// prepare the table;

$tableHTMLString = $table->prepare();


# echo $tableHTMLString;

```
