array_pagination
================
Example Usage:
//Creating dummy array.
for ($i = 1; $i <= 100; $i++)
{
	$array[] = "Result #$i";
}

//Getting currect page.
$page = $_GET['page'];

//Applying pagination.
$pagination = pagination_array($array, $page, "?page=");

//Page link panel.
echo $pagination['panel'];

//Displayed page results.
echo '<pre>';
print_r($pagination['array']);
echo '</pre>';

//Page link panel.
echo $pagination['panel'];

Original Source:
http://www.codehive.net/PHP-Array-Pagination-10.html
