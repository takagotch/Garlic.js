### Garlic.js
---
https://github.com/guillaumepotier/Garlic.js

```
<script src="jquery.js">
<script src="garlic.js">

<from data-persist="garlic" method="POST">
```

```js
$( '[rel=persist]' ).garlic();

$( 'input.no_good' ).garlic( 'destroy' );

$( 'input.no_good' ).garlic( {
  onPersist: function( elem, storedValue ){
    console.log( 'The persisted value for ' + elem.name() + ' is : ' + storedValue );
  }
} );

$( '#form' ).garlic( {
  getPath: function( $elem ){
    return $elem.attr( 'id' );
  }
} );
```

```
```

