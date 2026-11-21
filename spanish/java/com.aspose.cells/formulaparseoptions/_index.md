---
title: "FormulaParseOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa opciones al analizar la fórmula."
type: docs
url: /es/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

Representa opciones al analizar la fórmula.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | Indica si se deben comprobar los complementos en los enlaces externos existentes del libro actual para funciones definidas por el usuario sin enlace externo. |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | Definición para analizar funciones personalizadas. |
| [getLocaleDependent()](#getLocaleDependent--) | Si la fórmula está formateada según la configuración regional. |
| [getParse()](#getParse--) | Indica si se analiza la fórmula dada. |
| [getR1C1Style()](#getR1C1Style--) | Indica si la fórmula está en estilo de referencia R1C1. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | Indica si se deben comprobar los complementos en los enlaces externos existentes del libro actual para funciones definidas por el usuario sin enlace externo. |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Definición para analizar funciones personalizadas. |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | Si la fórmula está formateada según la configuración regional. |
| [setParse(boolean value)](#setParse-boolean-) | Indica si se analiza la fórmula dada. |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | Indica si la fórmula está en estilo de referencia R1C1. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
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
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


Indica si se deben comprobar los complementos en los enlaces externos existentes del libro actual para funciones definidas por el usuario sin enlace externo. El valor predeterminado es true (si la función definida por el usuario coincide con un complemento en los enlaces externos existentes, se toma como ese complemento).

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


Definición para analizar funciones personalizadas.

**Remarks**

Para algunos requisitos especiales, como al calcular una función personalizada en el motor personalizado del usuario, algunos de sus parámetros deben calcularse en modo matriz; usar esta propiedad puede marcar esos parámetros como modo matriz al analizar la fórmula. De lo contrario, el usuario debe actualizar esas funciones personalizadas más tarde mediante [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) para obtener el mismo resultado.

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


Indica si la fórmula está formateada según la configuración regional. El valor predeterminado es false.

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


Indica si se analiza la fórmula dada. El valor predeterminado es true. Si es false, la cadena de fórmula proporcionada se mantendrá tal cual en la celda hasta que el usuario llame a otros métodos para analizarla o se requieran datos de fórmula analizada por otras operaciones, como el cálculo de fórmulas.

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


Indica si la fórmula está en estilo de referencia R1C1. El valor predeterminado es false.

**Returns:**
boolean
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




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


Indica si se deben comprobar los complementos en los enlaces externos existentes del libro actual para funciones definidas por el usuario sin enlace externo. El valor predeterminado es true (si la función definida por el usuario coincide con un complemento en los enlaces externos existentes, se toma como ese complemento).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


Definición para analizar funciones personalizadas.

**Remarks**

Para algunos requisitos especiales, como al calcular una función personalizada en el motor personalizado del usuario, algunos de sus parámetros deben calcularse en modo matriz; usar esta propiedad puede marcar esos parámetros como modo matriz al analizar la fórmula. De lo contrario, el usuario debe actualizar esas funciones personalizadas más tarde mediante [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) para obtener el mismo resultado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


Indica si la fórmula está formateada según la configuración regional. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


Indica si se analiza la fórmula dada. El valor predeterminado es true. Si es false, la cadena de fórmula proporcionada se mantendrá tal cual en la celda hasta que el usuario llame a otros métodos para analizarla o se requieran datos de fórmula analizada por otras operaciones, como el cálculo de fórmulas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


Indica si la fórmula está en estilo de referencia R1C1. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

