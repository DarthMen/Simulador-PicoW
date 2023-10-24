# templete-picow
Para trabajos de microcontroladores
https://wokwi.com/projects/379512202156426241
```C
/*
 * Nombre del Archivo: PicoW Simulado.c
 * Autor:   [MIRANDA JUAREZ PAUL EMANUEL]
 * Correo:  [L21210401@tectijuana.edu.mx]
 * Fecha:   [23/10/2023]
 * Curso:   Lenguajes de Interfaz, TECNM Campus ITT
 * 
 * Objetivo:
 * Lograr encender un led y impirmir hola mundo (practicar).
 *
 * Historial de Revisiones:
 * [23/10/2023]        [MIRANDA JUAREZ PAUL EMANUEL] - Creado
 * [24/10/2023]        [MIRANDA JUAREZ PAUL EMANUEL] - Corregido [característica/corrección]
 *
 */

#include "pico/stdlib.h"
#include <stdio.h>

int main() {
    stdio_init_all();
    const uint LED_PIN = 25;
    gpio_init(LED_PIN);
    gpio_set_dir(LED_PIN, GPIO_OUT);

    while (1) {
        printf("Hola Mundo\n");
        gpio_put(LED_PIN, 1);  // Enciende el LED
        sleep_ms(1000);
        gpio_put(LED_PIN, 0);  // Apaga el LED
        sleep_ms(1000);
    }
}
```

# Evaluacion
• 100% DEPOSTAR EL URL de su Wokwi funcionando Incluir el templete del código sin el no se recibirán las practicas.
# Recursos
1.- https://wokwi.com/projects/379512202156426241
