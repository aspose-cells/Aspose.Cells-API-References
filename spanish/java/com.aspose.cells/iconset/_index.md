---
title: "IconSet"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Describe la regla de formato condicional IconSet."
type: docs
url: /es/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

Describe la regla de formato condicional IconSet. Esta regla de formato condicional aplica iconos a las celdas según sus valores.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Icon Set
         IconSet iconSet = cond.getIconSet();
 
         //Set Icon Type
         iconSet.setType(IconSetType.ARROWS_3);
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | Obtén el[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) de la colección |
| [getCfvos()](#getCfvos--) | Obtén la instancia de CFValueObjects. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | Obtiene la bandera que indica si se invierte el orden predeterminado de los iconos en este conjunto de iconos. |
| [getShowValue()](#getShowValue--) | Obtiene la bandera que indica si se muestran los valores de las celdas a las que se aplica este conjunto de iconos. |
| [getType()](#getType--) | Obtiene el tipo de conjunto de iconos a mostrar. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | Indica si el conjunto de iconos es personalizado. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | Establece la bandera que indica si se invierte el orden predeterminado de los iconos en este conjunto de iconos. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Establece la bandera que indica si se muestran los valores de las celdas a las que se aplica este conjunto de iconos. |
| [setType(int value)](#setType-int-) | Establece el tipo de conjunto de iconos a mostrar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


Obtén el[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) de la colección

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


Obtén la instancia de CFValueObjects.

**Returns:**
[ConditionalFormattingValueCollection](../../com.aspose.cells/conditionalformattingvaluecollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getReverse() {#getReverse--}
```
public boolean getReverse()
```


Obtiene la bandera que indica si se invierte el orden predeterminado de los iconos en este conjunto de iconos. El valor predeterminado es falso.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Obtiene la bandera que indica si se muestran los valores de las celdas a las que se aplica este conjunto de iconos. El valor predeterminado es verdadero.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de conjunto de iconos a mostrar. Configurar el tipo comprobará automáticamente si el recuento actual de Cfods coincide con el nuevo tipo. Si no coincide, los Cfods antiguos se eliminarán y se añadirán los Cfods predeterminados.

Ver [IconSetType](../../com.aspose.cells/iconsettype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCustom() {#isCustom--}
```
public boolean isCustom()
```


Indica si el conjunto de iconos es personalizado. El valor predeterminado es falso.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setReverse(boolean value) {#setReverse-boolean-}
```
public void setReverse(boolean value)
```


Establece la bandera que indica si se invierte el orden predeterminado de los iconos en este conjunto de iconos. El valor predeterminado es falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Establece la bandera que indica si se muestran los valores de las celdas a las que se aplica este conjunto de iconos. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Establece el tipo de conjunto de iconos a mostrar. Al establecer el tipo, se verificará automáticamente si el recuento actual de Cfvos coincide con el nuevo tipo. Si no coincide, los Cfvos antiguos se limpiarán y se agregarán los Cfvos predeterminados.

Ver [IconSetType](../../com.aspose.cells/iconsettype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

