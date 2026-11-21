---
title: "CustomFunctionDefinition"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Definición de función personalizada para calcular con el motor personalizado del usuario."
type: docs
url: /es/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

Definición de función personalizada para calcular con el motor personalizado del usuario.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | Obtiene los índices de los parámetros de la función personalizada dada que deben calcularse en modo de matriz. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFunctionDefinition() {#CustomFunctionDefinition--}
```
public CustomFunctionDefinition()
```


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
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


Obtiene los índices de los parámetros de la función personalizada dada que deben calcularse en modo de matriz.

**Remarks**

Para una expresión que necesita ser calculada, tomando A:A+B:B como ejemplo: generalmente en modo valor se calculará a un solo valor según la base de la celda actual. Pero en modo matriz, todos los valores de A1+B1, A2+B2, A3+B3, ... se calcularán y se usarán para el cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionName | java.lang.String | Nombre de la función personalizada. |

**Returns:**
int[] - Índices de los parámetros que deben calcularse en modo de matriz para la función personalizada dada. El valor predeterminado es null, no hay ningún parámetro que necesite calcularse en modo de matriz para la función personalizada.
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

