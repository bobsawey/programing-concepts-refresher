# Personal Programming Concepts Refresher

## OOP
### Terms
#### Lifetime :
> In object-oriented programming (OOP), the object lifetime (or life cycle) of an object is the time between an object's creation > and its destruction. Rules for object lifetime vary significantly between languages, in some cases between implementations of a > given language, and lifetime of a particular object may vary from one run of the program to another.

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
