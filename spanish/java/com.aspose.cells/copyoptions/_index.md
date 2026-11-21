---
title: "CopyOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de copia."
type: docs
url: /es/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

Representa las opciones de copia.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | Constructor de CopyOptions. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Indica si se copia el ancho de columna en unidades de caracteres. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | Si la fórmula no es válida para el destino, solo se copian los valores. |
| [getCopyNames()](#getCopyNames--) | Indica si se copian los nombres. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Indica si se extienden los rangos al copiar el rango a un rango adyacente. |
| [getKeepMacros()](#getKeepMacros--) | Indica si se conservan las macros; |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | Al copiar el rango en el mismo archivo y el gráfico hace referencia a la hoja de origen, False significa que la fuente de datos del gráfico copiado no se modificará. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | En MS Excel, al copiar fórmulas que hacen referencia a otras hojas mientras se copia una hoja a otra, las fórmulas copiadas deben referirse al libro de origen. |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | Indica si se debe referir a la hoja de destino cuando la hoja referenciada no se copia. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | Indica si se copia el ancho de columna en unidades de caracteres. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | Si la fórmula no es válida para el destino, solo se copian los valores. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | Indica si se copian los nombres. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | Indica si se extienden los rangos al copiar el rango a un rango adyacente. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | Indica si se conservan las macros; |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | Al copiar el rango en el mismo archivo y el gráfico hace referencia a la hoja de origen, False significa que la fuente de datos del gráfico copiado no se modificará. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | En MS Excel, al copiar fórmulas que hacen referencia a otras hojas mientras se copia una hoja a otra, las fórmulas copiadas deben referirse al libro de origen. |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | Indica si se debe referir a la hoja de destino cuando la hoja referenciada no se copia. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


Constructor de CopyOptions.

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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


Indica si se copia el ancho de columna en unidades de caracteres.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


Si la fórmula no es válida para el destino, solo se copian los valores.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


Indica si se copian los nombres.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


Indica si se extienden los rangos al copiar el rango a un rango adyacente.

**Remarks**

Si es true, solo amplía el rango del hipervínculo, sin añadir un nuevo hipervínculo al copiar hipervínculos a filas adyacentes.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


Indica si se conservan las macros;

**Remarks**

Solo para copiar el libro de trabajo.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


Al copiar el rango en el mismo archivo y el gráfico hace referencia a la hoja de origen, False significa que la fuente de datos del gráfico copiado no se modificará. True indica que la fuente de datos del gráfico copiado hace referencia a la hoja de destino.

**Remarks**

El valor predeterminado es false, funciona como MS Excel. Por ejemplo: si se copia un gráfico con la fuente de datos "sheet1!A1:B10" de la hoja "sheet1" a otra hoja "sheet2", la fuente de datos se cambiará a "sheet2!A1:B10"

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


En MS Excel, al copiar fórmulas que hacen referencia a otras hojas mientras se copia una hoja a otra, las fórmulas copiadas deben referirse al libro de origen. Sin embargo, en algunas situaciones el usuario puede necesitar que las fórmulas copiadas se refieran a hojas con el mismo nombre en el mismo libro, como cuando esas hojas ya fueron copiadas antes de esta operación, entonces esta propiedad debe mantenerse en true.

**Remarks**

El valor predeterminado es true.

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


Indica si se debe referir a la hoja de destino cuando la hoja referenciada no se copia.

**Remarks**

Solo funciona al copiar rangos o hojas de cálculo desde otro obook.

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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


Indica si se copia el ancho de columna en unidades de caracteres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


Si la fórmula no es válida para el destino, solo se copian los valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


Indica si se copian los nombres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


Indica si se extienden los rangos al copiar el rango a un rango adyacente.

**Remarks**

Si es true, solo amplía el rango del hipervínculo, sin añadir un nuevo hipervínculo al copiar hipervínculos a filas adyacentes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


Indica si se conservan las macros;

**Remarks**

Solo para copiar el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


Al copiar el rango en el mismo archivo y el gráfico hace referencia a la hoja de origen, False significa que la fuente de datos del gráfico copiado no se modificará. True indica que la fuente de datos del gráfico copiado hace referencia a la hoja de destino.

**Remarks**

El valor predeterminado es false, funciona como MS Excel. Por ejemplo: si se copia un gráfico con la fuente de datos "sheet1!A1:B10" de la hoja "sheet1" a otra hoja "sheet2", la fuente de datos se cambiará a "sheet2!A1:B10"

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


En MS Excel, al copiar fórmulas que hacen referencia a otras hojas mientras se copia una hoja a otra, las fórmulas copiadas deben referirse al libro de origen. Sin embargo, en algunas situaciones el usuario puede necesitar que las fórmulas copiadas se refieran a hojas con el mismo nombre en el mismo libro, como cuando esas hojas ya fueron copiadas antes de esta operación, entonces esta propiedad debe mantenerse en true.

**Remarks**

El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


Indica si se debe referir a la hoja de destino cuando la hoja referenciada no se copia.

**Remarks**

Solo funciona al copiar rangos o hojas de cálculo desde otro obook.

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

