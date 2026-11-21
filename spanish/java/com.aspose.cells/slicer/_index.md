---
title: "Segmentador"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "descripción resumida de Slicer View"
type: docs
url: /es/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

descripción resumida de Slicer View

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
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | Agrega una conexión de tabla dinámica. |
| [clearFilter()](#clearFilter--) | Eliminar filtros |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto Slicer. |
| [getCaption()](#getCaption--) | Devuelve o establece el título del slicer especificado. |
| [getCaptionVisible()](#getCaptionVisible--) | Devuelve o establece si la cabecera que muestra el título del slicer es visible. |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | Devuelve o establece el ancho de cada columna en el slicer en unidades de puntos. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | Obtiene el ancho de\u807deach column in\u807dthe slicer, en unidades de\u807dpixels.\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | Especifica el índice basado en cero del primer elemento del slicer. |
| [getHeight()](#getHeight--) | Devuelve o establece la altura del slicer especificado, en puntos. |
| [getHeightPixel()](#getHeightPixel--) | Devuelve o establece la altura del slicer especificado, en píxeles. |
| [getLeftPixel()](#getLeftPixel--) | Devuelve o establece el desplazamiento horizontal de la forma del slicer desde su columna izquierda, en píxeles. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | Indica si la relación de aspecto está bloqueada. |
| [getLockedPosition()](#getLockedPosition--) | Indica si el slicer especificado puede moverse o redimensionarse mediante la interfaz de usuario. |
| [getName()](#getName--) | Devuelve o establece el nombre del slicer especificado |
| [getNumberOfColumns()](#getNumberOfColumns--) | Devuelve o establece el número de columnas en el slicer. |
| [getParent()](#getParent--) | Devuelve el objeto [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) que contiene este slicer. |
| [getPlacement()](#getPlacement--) | Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. |
| [getRowHeight()](#getRowHeight--) | Devuelve o establece la altura de cada fila en el slicer especificado en unidades de puntos. |
| [getRowHeightPixel()](#getRowHeightPixel--) | Devuelve o establece la altura de cada fila en el slicer especificado, en unidades de píxeles. |
| [getShape()](#getShape--) | Devuelve el objeto Shape asociado con el slicer especificado. |
| [getShowAllItems()](#getShowAllItems--) | Indica si se deben mostrar todos los elementos aunque no haya datos o hayan sido eliminados. |
| [getShowCaption()](#getShowCaption--) | Indica si el encabezado del slicer es visible. |
| [getShowMissing()](#getShowMissing--) | Indica si se deben mostrar los elementos eliminados de la fuente de datos. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | Indica si se deben mostrar los elementos eliminados de la fuente de datos. |
| [getSlicerCache()](#getSlicerCache--) | Devuelve el objeto SlicerCache asociado con el slicer. |
| [getSortOrderType()](#getSortOrderType--) | Indica el tipo de ordenamiento de los elementos. |
| [getStyleType()](#getStyleType--) | Especifique el tipo de estilo incorporado del slicer. |
| [getTitle()](#getTitle--) | Especifica el título del objeto Slicer actual. |
| [getTopPixel()](#getTopPixel--) | Devuelve o establece el desplazamiento vertical de la forma del slicer desde su fila superior, en píxeles. |
| [getWidth()](#getWidth--) | Devuelve o establece el ancho del slicer especificado, en puntos. |
| [getWidthPixel()](#getWidthPixel--) | Devuelve o establece el ancho del slicer especificado, en píxeles. |
| [getWorksheet()](#getWorksheet--) | Devuelve el objeto [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) que contiene este slicer. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | Indica si la forma del slicer está bloqueada. |
| [isPrintable()](#isPrintable--) | Indica si el objeto slicer es imprimible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Actualizando los elementos del slicer desde las tablas dinámicas asociadas. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | Elimina la conexión de la tabla dinámica. |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **Observaciones** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto Slicer. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Devuelve o establece el título del slicer especificado. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | Devuelve o establece si la cabecera que muestra el título del slicer es visible. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Devuelve o establece el ancho de cada columna en el slicer en unidades de puntos. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | Establece el ancho de\u807deach column in\u807dthe slicer, en unidades de\u807dpixels.\u807d |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | Especifica el índice basado en cero del primer elemento del slicer. |
| [setHeight(double value)](#setHeight-double-) | Devuelve o establece la altura del slicer especificado, en puntos. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Devuelve o establece la altura del slicer especificado, en píxeles. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Devuelve o establece el desplazamiento horizontal de la forma del slicer desde su columna izquierda, en píxeles. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indica si la forma del slicer está bloqueada. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | Indica si la relación de aspecto está bloqueada. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | Indica si el slicer especificado puede moverse o redimensionarse mediante la interfaz de usuario. |
| [setName(String value)](#setName-java.lang.String-) | Devuelve o establece el nombre del slicer especificado |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Devuelve o establece el número de columnas en el slicer. |
| [setPlacement(int value)](#setPlacement-int-) | Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Indica si el objeto slicer es imprimible. |
| [setRowHeight(double value)](#setRowHeight-double-) | Devuelve o establece la altura de cada fila en el slicer especificado en unidades de puntos. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | Devuelve o establece la altura de cada fila en el slicer especificado, en unidades de píxeles. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Indica si se deben mostrar todos los elementos aunque no haya datos o hayan sido eliminados. |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | Indica si el encabezado del slicer es visible. |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | Indica si se deben mostrar los elementos eliminados de la fuente de datos. |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | Indica si se deben mostrar los elementos eliminados de la fuente de datos. |
| [setSortOrderType(int value)](#setSortOrderType-int-) | Indica el tipo de ordenamiento de los elementos. |
| [setStyleType(int value)](#setStyleType-int-) | Especifique el tipo de estilo incorporado del slicer. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Especifica el título del objeto Slicer actual. |
| [setTopPixel(int value)](#setTopPixel-int-) | Devuelve o establece el desplazamiento vertical de la forma del slicer desde su fila superior, en píxeles. |
| [setWidth(double value)](#setWidth-double-) | Devuelve o establece el ancho del slicer especificado, en puntos. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Devuelve o establece el ancho del slicer especificado, en píxeles. |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | Eliminar etiquetas de filtro seleccionadas. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


Agrega una conexión de tabla dinámica.

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | El objeto PivotTable |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Eliminar filtros

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto Slicer.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.getAlternativeText()](../../com.aspose.cells/shape\\#getAlternativeText--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


Devuelve o establece el título del slicer especificado.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


Devuelve o establece si el encabezado que muestra el título del segmentador es visible. El valor predeterminado es true

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [getShowCaption()](../../com.aspose.cells/slicer\\#getShowCaption--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Devuelve o establece el ancho de cada columna en el slicer en unidades de puntos.

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


Obtiene el ancho de\u807deach column in\u807dthe slicer, en unidades de\u807dpixels.\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


Especifica el índice basado en cero del primer elemento del slicer.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Devuelve o establece la altura del slicer especificado, en puntos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.HeightPt. Esta propiedad será eliminada 12 meses después a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Devuelve o establece la altura del slicer especificado, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Height. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Devuelve o establece el desplazamiento horizontal de la forma del slicer desde su columna izquierda, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Left. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


Indica si la relación de aspecto está bloqueada.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\\#isAspectRatioLocked--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


Indica si el slicer especificado puede moverse o redimensionarse mediante la interfaz de usuario.

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Devuelve o establece el nombre del slicer especificado

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Devuelve o establece el número de columnas en el segmentador. El valor predeterminado es 1.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


Devuelve el objeto [getWorksheet()](../../com.aspose.cells/slicer\\#getWorksheet--) que contiene este segmentador. Solo lectura.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [getWorksheet()](../../com.aspose.cells/slicer\\#getWorksheet--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de cálculo.

Ver [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.getPlacement()](../../com.aspose.cells/shape\\#getPlacement--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Devuelve o establece la altura de cada fila en el slicer especificado en unidades de puntos.

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


Devuelve o establece la altura de cada fila en el slicer especificado, en unidades de píxeles.

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


Devuelve el objeto Shape asociado con el segmentador especificado. Solo lectura.

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indica si se deben mostrar todos los elementos incluso si no hay datos o están eliminados. El valor predeterminado es true;

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


Indica si el encabezado del segmentador es visible. El valor predeterminado es true

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


Indica si se deben mostrar los elementos eliminados de la fuente de datos.

**Remarks**

Solo funciona cuando [getShowAllItems()](../../com.aspose.cells/slicer\\#getShowAllItems--) es true.

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


Indica si se deben mostrar los elementos eliminados de la fuente de datos.

Vea [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Solo funciona cuando [getShowAllItems()](../../com.aspose.cells/slicer\\#getShowAllItems--) es true.

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


Devuelve el objeto SlicerCache asociado con el segmentador. Solo lectura.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


Indica el tipo de ordenamiento de los elementos.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


Especifique el tipo de estilo de segmentador incorporado. El tipo predeterminado es SlicerStyleLight1.

Vea [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


Especifica el título del objeto Slicer actual.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.getTitle()](../../com.aspose.cells/shape\\#getTitle--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Devuelve o establece el desplazamiento vertical de la forma del slicer desde su fila superior, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Top. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Devuelve o establece el ancho del slicer especificado, en puntos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.WidthPt. Esta propiedad será eliminada 12 meses después a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Devuelve o establece el ancho del slicer especificado, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Width. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Devuelve el objeto [getWorksheet()](../../com.aspose.cells/slicer\\#getWorksheet--) que contiene este segmentador. Solo lectura.

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Indica si la forma del slicer está bloqueada.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.isLocked()](../../com.aspose.cells/shape\\#isLocked--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Indica si el objeto slicer es imprimible.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.isPrintable()](../../com.aspose.cells/shape\\#isPrintable--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Example**

```
         slicer.removePivotConnection(pivot);
```

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




### refresh() {#refresh--}
```
public void refresh()
```


Actualizando los elementos del slicer desde las tablas dinámicas asociadas.

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


Elimina la conexión de la tabla dinámica.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | El objeto PivotTable |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

Si desea seleccionar todos los elementos, utilice el método [clearFilter()](../../com.aspose.cells/slicer\\#clearFilter--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| etiquetas | java.lang.String[] | Etiquetas seleccionadas. |
| añadir | boolean | False significa que solo se seleccionan estas etiquetas y se deseleccionan las demás. True significa que se conservan los elementos seleccionados anteriormente y se seleccionan estas etiquetas. |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto Slicer.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.getAlternativeText()](../../com.aspose.cells/shape\\#getAlternativeText--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Devuelve o establece el título del slicer especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


Devuelve o establece si el encabezado que muestra el título del segmentador es visible. El valor predeterminado es true

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [getShowCaption()](../../com.aspose.cells/slicer\\#getShowCaption--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Devuelve o establece el ancho de cada columna en el slicer en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


Establece el ancho de\u807deach column in\u807dthe slicer, en unidades de\u807dpixels.\u807d

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


Especifica el índice basado en cero del primer elemento del slicer.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Devuelve o establece la altura del slicer especificado, en puntos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.HeightPt. Esta propiedad será eliminada 12 meses después a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Devuelve o establece la altura del slicer especificado, en píxeles.

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


Devuelve o establece el desplazamiento horizontal de la forma del slicer desde su columna izquierda, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Left. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indica si la forma del slicer está bloqueada.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.isLocked()](../../com.aspose.cells/shape\\#isLocked--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


Indica si la relación de aspecto está bloqueada.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\\#isAspectRatioLocked--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


Indica si el slicer especificado puede moverse o redimensionarse mediante la interfaz de usuario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Devuelve o establece el nombre del slicer especificado

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Devuelve o establece el número de columnas en el segmentador. El valor predeterminado es 1.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de cálculo.

Ver [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.getPlacement()](../../com.aspose.cells/shape\\#getPlacement--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Indica si el objeto slicer es imprimible.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.isPrintable()](../../com.aspose.cells/shape\\#isPrintable--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Devuelve o establece la altura de cada fila en el slicer especificado en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


Devuelve o establece la altura de cada fila en el slicer especificado, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Indica si se deben mostrar todos los elementos incluso si no hay datos o están eliminados. El valor predeterminado es true;

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


Indica si el encabezado del segmentador es visible. El valor predeterminado es true

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


Indica si se deben mostrar los elementos eliminados de la fuente de datos.

**Remarks**

Solo funciona cuando [getShowAllItems()](../../com.aspose.cells/slicer\\#getShowAllItems--) es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


Indica si se deben mostrar los elementos eliminados de la fuente de datos.

Vea [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Solo funciona cuando [getShowAllItems()](../../com.aspose.cells/slicer\\#getShowAllItems--) es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


Indica el tipo de ordenamiento de los elementos.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


Especifique el tipo de estilo de segmentador incorporado. El tipo predeterminado es SlicerStyleLight1.

Vea [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Especifica el título del objeto Slicer actual.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [Shape.getTitle()](../../com.aspose.cells/shape\\#getTitle--). Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Devuelve o establece el desplazamiento vertical de la forma del slicer desde su fila superior, en píxeles.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Top. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Devuelve o establece el ancho del slicer especificado, en puntos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.WidthPt. Esta propiedad será eliminada 12 meses después a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Devuelve o establece el ancho del slicer especificado, en píxeles.

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
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


Eliminar etiquetas de filtro seleccionadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| etiquetas | java.lang.String[] | Las etiquetas. |

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

