#PHP for WordPress Developers
By The Atlanta WordPress Coder's Guild

##PHP Basics 

###Comments
	// Single line Comment

	/*
	 * Multiline Comment
	 */

	/**
	 * PHPDoc Comment 
	 */
	 
###Literal Values
	1
	'hello'
	true
	
##Output and Types
	echo <value>;
	
	echo 1;			// Integer Number
	echo 3.14159;	// Floating Point Number
	echo 'hello';	// String
	echo false;		// Boolean
		
###Variables
	$variable = <value>;
	
	$num = 10;

	global <variable>;
	
###Expressions and Values
	echo ! $done;
	
	$count = 1;
	$count = $count + 1;
	$count = $count - 5;
	
	$count = ( $count + 9 ) * 10;
	$count = $count / 2;
	
	$is_30 = 30 == $count;
	$is_not_30 = ! $is_30;

	$alway = $is_30 || $is_not_30;
	$never = $is_30 && $is_not_30;
	
###Constants
	define( 'CONSTANT', <value> );

	define( 'WP_DEBUG', true );
	define( 'WP_HOME', 'http://example.php' );
	
	echo WP_DEBUG;
	echo WP_HOME;	

###Branching - IF
	if ( <expression> ) { 

		<statement>
		
	}

	if ( <expression> ) { 

		<if-true-statement>

	} else {
		
		<if-false-statement>

	}
	
	if ( <expr1> ) { 

		<if-expr1-is-true-statement>

	} else if ( <expr2> ) {
		
		<if-expr2-is-true-statement>

	} else {
	
		<if-not-expr1-or-expr2>

	}

###Arrays
	array( <element-1>, <element-2>, ... <element-n> );
	
	$numbers = array( 1, 2, 3, );
	$letters = array( 'one',' two', 'three' );
	
	print_r( $numbers );
	print_r( $letters );
	
	array( 
		<key-1> => <value-1>, 
		<key-2> => <value-2>,
		<key-n> => <value-n>,
	);
		
	$favorite = array(
		'url'  		=> 'http://google.com',
		'link_text' => 'Google',
	);
	
	print_r( $favorite );


###Branching - SWITCH

	switch ( <expression> ) { 

		case <value-1>:
		
			<case-value1-statement>
			break;

		case <value-2>:
				
			<case-value2-statement>
			break;

		case <value-3>:

			<case-value3-statement>
			break;

		default:		

			<case-not-value1-value2-value3-statement>
			break;

	}

###Functions

	function <name>( <param-1>, <param-2>, ... <param-n> ) {

		<statements>

		return <value;	
	
	}
	
	