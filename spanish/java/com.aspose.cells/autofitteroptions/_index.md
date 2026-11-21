---
title: "AutoFitterOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todas las opciones de ajuste automático."
type: docs
url: /es/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

Representa todas las opciones de ajuste automático.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Indica si se ajusta automáticamente la altura de la fila cuando las celdas están combinadas en una fila. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | Obtiene el tipo de ajuste automático de la altura de fila de celdas combinadas. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | Obtiene el tipo de ajuste automático del texto envuelto. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Obtiene el idioma de edición predeterminado. |
| [getForRendering()](#getForRendering--) | Indica si se ajusta para propósitos de renderizado. |
| [getFormatStrategy()](#getFormatStrategy--) | Obtiene la estrategia de formato. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Ignora las filas/columnas ocultas. |
| [getMaxRowHeight()](#getMaxRowHeight--) | Obtiene la altura máxima de fila (en unidades de Punto) al ajustar automáticamente las filas. |
| [getOnlyAuto()](#getOnlyAuto--) | Indica si solo se ajustan las filas cuya altura no está personalizada. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | Indica si se ajusta automáticamente la altura de la fila cuando las celdas están combinadas en una fila. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | Establece el tipo de ajuste automático de la altura de fila de celdas combinadas. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | Establece el tipo de ajuste automático del texto ajustado. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Establece el idioma de edición predeterminado. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | Indica si se ajusta para propósitos de renderizado. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Establece la estrategia de formato. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | Ignora las filas/columnas ocultas. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | Establece la altura máxima de fila (en unidades de punto) al ajustar automáticamente las filas. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indica si solo se ajustan las filas cuya altura no está personalizada. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


Indica si se ajusta automáticamente la altura de fila cuando las celdas están combinadas en una fila. El valor predeterminado es false.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad AutoFitterOptions.AutoFitMergedCellsType. Esta propiedad será eliminada 12 meses después desde diciembre de 2018. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


Obtiene el tipo de ajuste automático de la altura de fila de celdas combinadas.

Ver [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel, por defecto, ignora las celdas combinadas al ajustar la altura de fila, por lo que Aspose.Cells funciona como el valor predeterminado de MS Excel. Por favor, establezca este tipo para cambiar la forma de ajuste automático de la altura de fila de celdas combinadas.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


Obtiene el tipo de ajuste automático del texto envuelto.

Ver [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Obtiene el idioma de edición predeterminado.

Ver [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Puede mostrar/renderizar diferentes diseños para el párrafo de texto cuando se establece un idioma de edición diferente. El valor predeterminado es [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


Indica si se ajusta para propósitos de renderizado.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Obtiene la estrategia de formato.

Ver [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

El valor predeterminado es CellStyle por rendimiento.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


Ignora las filas/columnas ocultas.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


Obtiene la altura máxima de fila (en unidades de Punto) al ajustar automáticamente las filas.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Indica si solo se ajustan las filas cuya altura no está personalizada.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


Indica si se ajusta automáticamente la altura de fila cuando las celdas están combinadas en una fila. El valor predeterminado es false.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad AutoFitterOptions.AutoFitMergedCellsType. Esta propiedad será eliminada 12 meses después desde diciembre de 2018. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


Establece el tipo de ajuste automático de la altura de fila de celdas combinadas.

Ver [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel, por defecto, ignora las celdas combinadas al ajustar la altura de fila, por lo que Aspose.Cells funciona como el valor predeterminado de MS Excel. Por favor, establezca este tipo para cambiar la forma de ajuste automático de la altura de fila de celdas combinadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


Establece el tipo de ajuste automático del texto ajustado.

Ver [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Establece el idioma de edición predeterminado.

Ver [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Puede mostrar/renderizar diferentes diseños para el párrafo de texto cuando se establece un idioma de edición diferente. El valor predeterminado es [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


Indica si se ajusta para propósitos de renderizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Establece la estrategia de formato.

Ver [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

El valor predeterminado es CellStyle por rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


Ignora las filas/columnas ocultas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


Establece la altura máxima de fila (en unidades de punto) al ajustar automáticamente las filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Indica si solo se ajustan las filas cuya altura no está personalizada.

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

