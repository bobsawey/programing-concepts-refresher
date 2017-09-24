# Programming Concepts Refresher


## Iterative functions

### PHP

```

function factorial($number){ 

  if ($number < 2){ 
    return 1; 
  } 
  
  else{ 
    return ($number * factorial($number-1)); 
  } 

}

```
more elaborately:
```
// from https://www.elated.com/articles/php-recursive-functions/
<?php
 
function factorial( $n ) {
 
  // Base case
  if ( $n == 0 ) {
    echo "Base case: \$n = 0. Returning 1...<br>";
    return 1;
  }
 
  // Recursion
  echo "\$n = $n: Computing $n * factorial( " . ($n-1) . " )...<br>";
  $result = ( $n * factorial( $n-1 ) );
  echo "Result of $n * factorial( " . ($n-1) . " ) = $result. Returning $result...<br>";
  return $result;
}
 
echo "The factorial of 5 is: " . factorial( 5 );
 
?>

```
