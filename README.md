# php-tools
PHP tools I have created that have helped me in my career

 /**
 *
 * PHPDump provides 'pretty' markup for dumping args, arrays, objects, etc.
 *
 * @param $arg    (required) The evaluated argument
 * @param $fg     (string: default: ff0 'orange')   :: foreground color
 * @param $bg     (string: default: 333 'dark gray) :: background color
 * @param $escape (boolean: default true) :: escapes html entities for display
 *
 */

<h2>Usage</h2>

require 'PHPDumpSA.funcion';

// examples

// dump an argument
$x = 'my value';

phpdump($x); // standard colors
phpdump($x,'f00','fff'); // red text - white background

$x = mysqi_query('select * from table');
phpdump($x); // displays information about mysqli resource

$x = [];
phpdump($x); // displays array elements

$x = new Car();
phpdump($x); // displays class object properties
