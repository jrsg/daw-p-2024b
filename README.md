# Examen parcial 2021b

Una aseguradora nacional te ha contratado para que desarrolles una solución en su proceso de
cálculo de seguros de vida. Por cada cotización se debe calcular el costo anual de la póliza utilizando el siguiente procedimiento:

Empieza calculando _factor_

1. Si el cliente es hombre entonces _factor_ es igual a 4%, si es mujer entonces _factor_ es igual 3%
2. Si edad (sólo considerar el mes y año de nacimiento)
   * menor o igual a 25 años, factor + 0.5%
   * mayor a 25 y menor o igual a 45 años, factor + 1%
   * mayor a 45 y menor o igual a 65 años, factor + 1.5%
   * mayor a 65 años, factor + 2%   * 
3. Si tiene/tuvo padecimientos:
   * Restar 2% a factor si no tiene/tuvo.
   * Sumar 1% a factor por cada padecimiento

Ahora calcula el costo anual con la siguiente fórmula:

`costo anual = factor X importe a recibir`

Una vez calculado:

4. Si son 2 los beneficiarios, aumentar un 25%.
5. Si forma de pago es anual no aumenta, semestral aumenta 3%, trimestral aumenta 5%, mensual aumenta 7%.

## Criterios

1. El dato de costo anual se calcula correctamente siguiendo el procedimiento indicado (5 punto)
2. El resumen o confirmación de la información de la cotización cuenta con la siguiente información (2 puntos):
    1. Costo anual (importe)
    2. Forma de pago (texto)
    3. Nombre del cliente (texto)
    4. Edad (años)
    5. Sexo (hombre o mujer)
    6. Estado de residencia (texto)
    7. Padecimientos (separados por comas)
    8. Nombre del beneficiario 1 y 2 (texto)
    9. Importe a recibir (importe)
3. Los datos de nombre del asegurado, sexo, fecha de nacimiento, Estado de residencia, importe a recibir y el nombre de al menos 1 beneficiario son datos obligatorios, los cuales se valida su captura antes de mostrar el resumen y calcular el costo anual. Por cada dato obligatorio faltante, el programa lo reporta con un mensaje de error explícito (usa window.alert). (1.5 punto)
4. El dato de la "Edad del cliente" se calcula considerando el mes y año de la fecha de nacimiento. Asume que todos los años tienen la misma cantidad de días (1.5 punto)
