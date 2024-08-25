# České svátky v JSON formátu

České svátky (jmeniny a státní svátky) podle dnů v roce ve formátu JSON.

## Příklad použití v PHP:

```php
<?php
$jsonFile  = file_get_contents( __DIR__ . DIRECTORY_SEPARATOR . 'svatky.json' );
$array     = json_decode( $jsonFile, true );

// echo $array[ MĚSÍC ][ DEN ];
echo $array[12][31]; // Zobrazí svátek 31.12 'Silvestr'
echo $array[7][30];  // Zobrazí svátek 30.7  'Bořivoj'
echo $array[1][1];   // Zobrazí svátek 1.1   'Nový rok'
```

## Podpora

**České svátky** jsou **open source** a **zdarma**. Podpořte proto prosím práci autora :

**BTC**: `bc1q03v5la7uvcwxr7z4qn03ex6n5edju6zv4n6ppt`

## Licence

**České svátky v JSON** je open source software licencován pod [MIT license](https://tldrlegal.com/license/mit-license).