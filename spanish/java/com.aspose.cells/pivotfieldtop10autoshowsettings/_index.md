---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración Top 10 AutoShow para un campo dinámico."
type: docs
url: /es/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

Representa la configuración Top 10 AutoShow para un campo dinámico.

**Remarks**

En xls: Implementación de filtros top 10 en Xls mediante Top 10 AutoShow. En archivos ooxml: El formato de archivo ooxml subyacente admite Top10 AutoShow, pero la interfaz de usuario de Excel 2007 y posteriores solo brinda acceso a través del filtro Top10. Si no se requiere compatibilidad con XLS, se recomienda usar el filtro Top10 en su lugar.

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
 
          //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | Especifica el índice del campo de datos para la clasificación AutoShow. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | Indica si se aplica un filtro "Top 10 AutoShow" a este campo. |
| [isTop()](#isTop--) | Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indica si se aplica un filtro "Top 10 AutoShow" a este campo. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado. |
| [setRankBy(int value)](#setRankBy-int-) | Especifica el índice del campo de datos para la clasificación AutoShow. |
| [setTop(boolean value)](#setTop-boolean-) | Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente. |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


Especifica el índice del campo de datos para la clasificación AutoShow. Representa el índice del campo auto show. -1 significa el propio PivotField. Debe ser el índice de los campos de datos.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indica si se aplica un filtro "Top 10 AutoShow" a este campo.

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indica si se aplica un filtro "Top 10 AutoShow" a este campo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


Especifica el índice del campo de datos para la clasificación AutoShow. Representa el índice del campo auto show. -1 significa el propio PivotField. Debe ser el índice de los campos de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente.

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

