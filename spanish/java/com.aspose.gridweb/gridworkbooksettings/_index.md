---
title: "GridWorkbookSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración del libro de trabajo."
type: docs
url: /es/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

Representa la configuración del libro de trabajo.

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | constructor predeterminado |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Obtiene el autor del archivo. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Obtiene si se verifica el formato numérico personalizado al establecer Style.Custom. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Obtiene si se crea la cadena de fórmulas calculadas. |
| [getDate1904()](#getDate1904--) | Obtiene el valor que indica si el libro de trabajo usa el sistema de fechas 1904. |
| [getEnableMacros()](#getEnableMacros--) | Obtiene si se habilitan las macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja dentro de un libro de trabajo. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Obtiene si calcula completamente cada vez que se desencadena un cálculo. |
| [getIteration()](#getIteration--) | Obtiene si usa iteración para resolver referencias circulares. |
| [getMaxIteration()](#getMaxIteration--) | Obtiene el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Verdadero si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Obtiene si recalcula todas las fórmulas al abrir el archivo. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Establece el autor del archivo. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Establece si se verifica el formato de número personalizado al establecer Style.Custom. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Establece si se crea una cadena de fórmulas calculadas. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Establece el valor que representa si el libro de trabajo usa el sistema de fechas 1904. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Establece si se habilitan macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja en un libro de trabajo. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Establece si calcula completamente cada vez que se desencadena un cálculo. |
| [setIteration(boolean value)](#setIteration-boolean-) | Establece si usa iteración para resolver referencias circulares. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Establece el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Verdadero si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Establece si recalcula todas las fórmulas al abrir el archivo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


constructor predeterminado

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtiene el autor del archivo.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Obtiene si se verifica el formato numérico personalizado al establecer Style.Custom.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Obtiene si se crea una cadena de fórmulas calculadas. El valor predeterminado es false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Obtiene el valor que indica si el libro de trabajo usa el sistema de fechas 1904.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Obtiene si se habilitan las macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja dentro de un libro de trabajo.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Obtiene si calcula completamente cada vez que se desencadena un cálculo.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Obtiene si usa iteración para resolver referencias circulares.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Obtiene el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Verdadero si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

**Remarks**

Generalmente esos espacios y saltos de línea son solo para fines visuales; preservarlos o no no afecta el resultado calculado. Por consideraciones de rendimiento, si no hay un requisito especial, es mejor no preservarlos al procesar fórmulas.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Obtiene si recalcula todas las fórmulas al abrir el archivo.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Establece el autor del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Establece si se verifica el formato de número personalizado al establecer Style.Custom.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Establece si se crea una cadena de fórmulas calculadas. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Establece el valor que representa si el libro de trabajo usa el sistema de fechas 1904.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Establece si se habilitan macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja en un libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Establece si calcula completamente cada vez que se desencadena un cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Establece si usa iteración para resolver referencias circulares.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Establece el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Verdadero si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.

**Remarks**

Generalmente esos espacios y saltos de línea son solo para fines visuales; preservarlos o no no afecta el resultado calculado. Por consideraciones de rendimiento, si no hay un requisito especial, es mejor no preservarlos al procesar fórmulas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Establece si recalcula todas las fórmulas al abrir el archivo.

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

