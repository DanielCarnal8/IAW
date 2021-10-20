# Calculadora con PHP

## PARTE DE HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <title>FORMULARIO DE EJEMPLO</title>
    <h1>CALCULADORA</h1>
    <form action="registro.php" method="post">
        
        <p>
            <input type="text" name="num1">
            <select name="operacion">
                <option value="suma">suma</option>
                <option value="resta">resta</option>
            </select>
            <input type="text" name="num2">
            <input type="submit" value="calcular">
        </p>
    </form>

</body>
</html>
```

## PARTE DE PHP
```php
<?php

$calculo = $_POST["operacion"];
$num1 = $_POST["num1"];
$num2 = $_POST["num2"];

if ($calculo == "suma")
{
$resultado =$num1 + $num2;
}
else if ($calculo == "resta")
{
$resultado =$num1 - $num2;
}

echo "el resultado es de " .$resultado;

?>
```
