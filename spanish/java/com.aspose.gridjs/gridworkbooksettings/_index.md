---
title: "GridWorkbookSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración del libro de trabajo."
type: docs
url: /es/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Representa la configuración del libro de trabajo.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Obtiene el autor del archivo. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indica si se verifica el formato numérico personalizado al establecer Style.Custom, el valor predeterminado es false. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Indica si se crea la cadena de fórmulas calculadas. |
| [getDate1904()](#getDate1904--) | Obtiene un valor que representa si el libro de trabajo usa el sistema de fechas 1904. |
| [getEnableMacros()](#getEnableMacros--) | Habilitar macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja dentro de un libro. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Indica si se calcula completamente cada vez que se desencadena un cálculo. |
| [getIteration()](#getIteration--) | Indica si se usa iteración para resolver referencias circulares. |
| [getMaxIteration()](#getMaxIteration--) | Devuelve o establece el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Verdadero si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Indica si se deben recalcular todas las fórmulas al abrir el archivo. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Establece el autor del archivo. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Indica si se verifica el formato numérico personalizado al establecer Style.Custom, el valor predeterminado es false. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Indica si se crea la cadena de fórmulas calculadas. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Establece un valor que representa si el libro de trabajo usa el sistema de fechas 1904. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Habilitar macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja dentro de un libro. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Indica si se calcula completamente cada vez que se desencadena un cálculo. |
| [setIteration(boolean value)](#setIteration-boolean-) | Indica si se usa iteración para resolver referencias circulares. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Devuelve o establece el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Verdadero si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Indica si se deben recalcular todas las fórmulas al abrir el archivo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
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


Indica si se verifica el formato numérico personalizado al establecer Style.Custom, el valor predeterminado es false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, como mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una Excepción. Si la propiedad es falsa, aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro de trabajo en formato Excel más adelante. De lo contrario, podría producirse un error inesperado en el archivo Excel generado. El valor predeterminado es falso.

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


Indica si se crea una cadena de fórmulas calculadas. El valor predeterminado es falso.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Obtiene un valor que representa si el libro de trabajo usa el sistema de fechas 1904.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Habilitar macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja dentro de un libro.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Indica si se calcula completamente cada vez que se desencadena un cálculo.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Indica si se usa iteración para resolver referencias circulares.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Devuelve o establece el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Verdadero si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Indica si se recalculan todas las fórmulas al abrir el archivo. El valor predeterminado es verdadero.

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


Indica si se verifica el formato numérico personalizado al establecer Style.Custom, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, como mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una Excepción. Si la propiedad es falsa, aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro de trabajo en formato Excel más adelante. De lo contrario, podría producirse un error inesperado en el archivo Excel generado. El valor predeterminado es falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Indica si se crea una cadena de fórmulas calculadas. El valor predeterminado es falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Establece un valor que representa si el libro de trabajo usa el sistema de fechas 1904.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Habilitar macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja dentro de un libro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Indica si se calcula completamente cada vez que se desencadena un cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Indica si se usa iteración para resolver referencias circulares.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Devuelve o establece el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100.

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

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Indica si se recalculan todas las fórmulas al abrir el archivo. El valor predeterminado es verdadero.

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

