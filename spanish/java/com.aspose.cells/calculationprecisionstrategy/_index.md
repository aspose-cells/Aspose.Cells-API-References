---
title: "CalculationPrecisionStrategy"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Enumera estrategias para manejar la precisión del cálculo."
type: docs
url: /es/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

Enumera estrategias para manejar la precisión de cálculo. Debido al problema de precisión de la aritmética de punto flotante IEEE 754, algunas fórmulas \"aparentemente simples\" pueden no calcularse con el resultado esperado. Por ejemplo la fórmula \"=-0.45+0.43+0.02\", al calcular los operandos con el operador '+' directamente, el resultado no es cero. Para este tipo de problema de precisión, algunas estrategias especiales pueden proporcionar el resultado esperado.
## Campos

| Campo | Descripción |
| --- | --- |
| [DECIMAL](#DECIMAL) | Utiliza decimal como operandos cuando sea posible. |
| [NONE](#NONE) | No se aplicó ninguna estrategia en el cálculo. |
| [ROUND](#ROUND) | Redondea el resultado del cálculo de acuerdo con los dígitos significativos. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Utiliza decimal como operandos cuando es posible. Es la opción menos eficiente en cuanto a rendimiento.

### NONE {#NONE}
```
public static final int NONE
```


No se aplicó ninguna estrategia en el cálculo. Al calcular, simplemente use el valor double original como operando y devuelva el resultado directamente. Es la opción más eficiente en cuanto a rendimiento y aplicable en la mayoría de los casos.

### ROUND {#ROUND}
```
public static final int ROUND
```


Redondea el resultado del cálculo de acuerdo con los dígitos significativos.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

