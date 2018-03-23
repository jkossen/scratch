# Lussen (Loops)

Met loops kun je herhalende acties uitvoeren. Je kunt bijvoorbeeld voor elk item in een lijst met studenten hun voornaam op het scherm tonen.

In PHP zijn drie soorten loops beschikbaar: for, foreach en while.

Meer informatie:
* https://www.w3schools.com/php/php_looping.asp
* https://secure.php.net/manual/en/control-structures.for.php
* https://secure.php.net/manual/en/control-structures.foreach.php
* https://secure.php.net/manual/en/control-structures.while.php

## foreach: door een array heen lopen

```php
<pre>
<?php
$my_arr = [
    'naam' => 'Jochem',
    'leeftijd' => 37,
    'woonplaats' => 'Zwolle'
];

/**
 * print elke key en waarde van $my_arr op het scherm
 */
foreach ($my_arr as $key => $value) {
    echo "$key=$value\n"; // \n is een newline (volgende regel)
}
```

## for: tien maal 'Ik ga thuis oefenen met PHP' op het scherm tonen

```php
<pre>
<?php

for ($i = 0; $i < 10; $i++) {
    echo "Ik ga thuis oefenen met PHP\n";
}
```

## while: zoek "Hans" in een lijst met namen

```php
<?php

$lijst = ["Jochem", "Arjan", "Hans", "Rémy"];
$zoek = 'Hans';
$found = false;
$pos = 0;

while (! $found) {
    if ($lijst[$pos] === $zoek) {
        $found = true;
    }

    $pos++;
}

if ($found) {
    echo "Ja, gevonden!";
}
```
