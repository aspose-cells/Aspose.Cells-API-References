---
title: "Timeline"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Descripción resumida de la vista Timeline Debido a que MS Excel 2003 no admite Timeline"
type: docs
url: /es/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

Descripción resumida de la vista Timeline. Debido a MS Excel, Excel 2003 no admite Timeline

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | Obtiene la leyenda de este Timeline. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | El nivel de tiempo actual del Timeline. |
| [getHeightPixel()](#getHeightPixel--) | Devuelve o establece la altura del timeline especificado, en píxeles. |
| [getLeftPixel()](#getLeftPixel--) | Devuelve o establece el desplazamiento horizontal de la forma del timeline desde su columna izquierda, en píxeles. |
| [getName()](#getName--) | Devuelve o establece el nombre del Timeline especificado |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | Obtiene el rango seleccionado de fecha y hora. |
| [getSelectionLevel()](#getSelectionLevel--) | Obtiene el nivel de tiempo en el que se realizó la selección actual para el Timeline. |
| [getShape()](#getShape--) | Devuelve el objeto [TimelineShape](../../com.aspose.cells/timelineshape) asociado a este Timeline. |
| [getShowHeader()](#getShowHeader--) | Indica si se muestra el encabezado de este timeline. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | Indica si se muestra la barra de desplazamiento horizontal. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | Indica si se muestra la etiqueta de selección. |
| [getShowTimeLevel()](#getShowTimeLevel--) | Indica si se muestra el cuadro de selección desplegable del nivel de tiempo. |
| [getStartDate()](#getStartDate--) | Obtiene la fecha de inicio de la posición de desplazamiento del intervalo de tiempo de este [Timeline](../../com.aspose.cells/timeline). |
| [getTopPixel()](#getTopPixel--) | Devuelve o establece el desplazamiento vertical de la forma del timeline desde su fila superior, en píxeles. |
| [getWidthPixel()](#getWidthPixel--) | Devuelve o establece el ancho del timeline especificado, en píxeles. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | Selecciona el elemento entre la fecha y hora. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Establece la leyenda de este Timeline. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | El nivel de tiempo actual del Timeline. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Devuelve o establece la altura del timeline especificado, en píxeles. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Devuelve o establece el desplazamiento horizontal de la forma del timeline desde su columna izquierda, en píxeles. |
| [setName(String value)](#setName-java.lang.String-) | Devuelve o establece el nombre del Timeline especificado |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | Establece el nivel de tiempo en el que se realizó la selección actual para el Timeline. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | Indica si se muestra el encabezado de este timeline. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | Indica si se muestra la barra de desplazamiento horizontal. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | Indica si se muestra la etiqueta de selección. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | Indica si se muestra el cuadro de selección desplegable del nivel de tiempo. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Establece la fecha de inicio de la posición de desplazamiento del intervalo de tiempo de este [Timeline](../../com.aspose.cells/timeline). |
| [setTopPixel(int value)](#setTopPixel-int-) | Devuelve o establece el desplazamiento vertical de la forma del timeline desde su fila superior, en píxeles. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Devuelve o establece el ancho del timeline especificado, en píxeles. |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


Obtiene la leyenda de este Timeline.

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


El nivel de tiempo actual del Timeline.

Ver [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Devuelve o establece la altura del timeline especificado, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Height. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Devuelve o establece el desplazamiento horizontal de la forma del timeline desde su columna izquierda, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Left. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Devuelve o establece el nombre del Timeline especificado

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


Obtiene el rango seleccionado de fecha y hora.

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


Obtiene el nivel de tiempo en el que se realizó la selección actual para el Timeline.

Ver [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


Devuelve el objeto [TimelineShape](../../com.aspose.cells/timelineshape) asociado a este Timeline.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


Indica si se muestra el encabezado de este timeline.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


Indica si se muestra la barra de desplazamiento horizontal.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


Indica si se muestra la etiqueta de selección.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


Indica si se muestra el cuadro de selección desplegable del nivel de tiempo.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Obtiene la fecha de inicio de la posición de desplazamiento del intervalo de tiempo de este [Timeline](../../com.aspose.cells/timeline).

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Devuelve o establece el desplazamiento vertical de la forma del timeline desde su fila superior, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Top. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Devuelve o establece el ancho del timeline especificado, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Width. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


Selecciona el elemento entre la fecha y hora.

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | La fecha y hora de inicio |
| end | [DateTime](../../com.aspose.cells/datetime) | La fecha y hora de fin |
| calcular | boolean | Indica si se deben calcular tablas dinámicas relativas |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Establece la leyenda de este Timeline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


El nivel de tiempo actual del Timeline.

Ver [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Devuelve o establece la altura del timeline especificado, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Height. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Devuelve o establece el desplazamiento horizontal de la forma del timeline desde su columna izquierda, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Left. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Devuelve o establece el nombre del Timeline especificado

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


Establece el nivel de tiempo en el que se realizó la selección actual para el Timeline.

Ver [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


Indica si se muestra el encabezado de este timeline.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


Indica si se muestra la barra de desplazamiento horizontal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


Indica si se muestra la etiqueta de selección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


Indica si se muestra el cuadro de selección desplegable del nivel de tiempo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Establece la fecha de inicio de la posición de desplazamiento del intervalo de tiempo de este [Timeline](../../com.aspose.cells/timeline).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Devuelve o establece el desplazamiento vertical de la forma del timeline desde su fila superior, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Top. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Devuelve o establece el ancho del timeline especificado, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Width. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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

