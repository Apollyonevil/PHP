<?php
// Genera un número aleatorio entre 1 y 100
$numero_secreto = rand(1, 100);
$intentos = 0;

echo "¡Bienvenido al juego de Adivina el Número!\n";
echo "Estoy pensando en un número entre 1 y 100. ¿Puedes adivinar cuál es?\n";

while (true) {
    echo "Introduce tu intento: ";
    $intento = trim(fgets(STDIN)); // Lee entrada del usuario
    $intentos++;

    if (!is_numeric($intento)) {
        echo "Por favor, introduce un número válido.\n";
        continue;
    }

    if ($intento < $numero_secreto) {
        echo "Demasiado bajo. ¡Intenta de nuevo!\n";
    } elseif ($intento > $numero_secreto) {
        echo "Demasiado alto. ¡Intenta de nuevo!\n";
    } else {
        echo "¡Felicidades! Has adivinado el número {$numero_secreto} en {$intentos} intentos.\n";
        break;
    }
}
?>
