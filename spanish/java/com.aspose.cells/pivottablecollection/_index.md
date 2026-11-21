---
title: "PivotTableCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la colección de todos los objetos PivotTable en la hoja de cálculo especificada."
type: docs
url: /es/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

Representa la colección de todos los objetos PivotTable en la hoja de cálculo especificada.

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
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Agrega una nueva tabla dinámica basada en otra tabla dinámica. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Agrega una nueva tabla dinámica basada en otra tabla dinámica. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | Agrega una nueva tabla dinámica moderna (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas. |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | Agrega una nueva tabla dinámica en la fila y columna especificadas de la hoja de cálculo. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003. |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | Agrega una nueva tabla dinámica moderna (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas. |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | Agrega una nueva tabla dinámica moderna (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003. |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003. |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | Agrega una nueva tabla dinámica. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | Agrega un nuevo objeto de tabla dinámica a la colección con múltiples rangos de consolidación como fuente de datos. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | Agrega un nuevo objeto de tabla dinámica a la colección con múltiples rangos de consolidación como fuente de datos. |
| [clear()](#clear--) | Borra todas las tablas dinámicas. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el informe de PivotTable por índice. |
| [get(int row, int column)](#get-int-int-) | Obtiene el [PivotTable](../../com.aspose.cells/pivottable) ubicado en la celda. |
| [get(String name)](#get-java.lang.String-) | Obtiene el informe de PivotTable por el nombre del PivotTable. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | Elimina el PivotTable especificado y elimina los datos del PivotTable. |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | Elimina el PivotTable especificado. |
| [removeAt(int index)](#removeAt-int-) | Elimina el PivotTable en el índice especificado y elimina los datos del PivotTable. |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | Elimina el PivotTable en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


Agrega una nueva tabla dinámica basada en otra tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | El PivotTable de origen. |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice del nuevo PivotTable añadido.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


Agrega una nueva tabla dinámica basada en otra tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | El PivotTable de origen. |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice del nuevo PivotTable añadido.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


Agrega una nueva tabla dinámica moderna (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| fila | int | El índice de fila basado en cero de la esquina superior izquierda del destino del PivotTable. |
| columna | int | El índice de columna basado en cero de la esquina superior izquierda del destino del PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


Agrega una nueva tabla dinámica en la fila y columna especificadas de la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| fila | int | El índice de fila basado en cero de la esquina superior izquierda del destino del PivotTable. |
| columna | int | El índice de columna basado en cero de la esquina superior izquierda del destino del PivotTable. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Opciones de creación de PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

**Remarks**

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de septiembre de 2026. Disculpe cualquier inconveniente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice en esta lista de pivot tables.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

**Remarks**

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de septiembre de 2026. Disculpe cualquier inconveniente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |
| useSameSource | boolean | Indica si se utiliza la misma fuente de datos cuando otra tabla dinámica existente ya ha usado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria. |

**Returns:**
int - El índice de caché añadido.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

**Remarks**

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de octubre de 2026. Disculpas por cualquier inconveniente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |
| useSameSource | boolean | Indica si se utiliza la misma fuente de datos cuando otra tabla dinámica existente ya ha usado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria. |
| isXlsClassic | boolean | Indica si se agrega una tabla dinámica clásica de Excel 97-2003. |

**Returns:**
int - El índice de caché añadido.
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


Agrega una nueva tabla dinámica moderna (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| cellName | java.lang.String | El nombre de la celda de la esquina superior izquierda para el destino de la tabla dinámica. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


Agrega una nueva tabla dinámica moderna (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| cellName | java.lang.String | El nombre de la celda de la esquina superior izquierda para el destino de la tabla dinámica. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Las opciones para crear la tabla dinámica. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

**Remarks**

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de septiembre de 2026. Disculpe cualquier inconveniente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | Los datos para la nueva caché de tabla dinámica. |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice en esta lista de pivot tables.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

**Remarks**

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de septiembre de 2026. Disculpe cualquier inconveniente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | Los datos para la nueva caché de tabla dinámica. |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |
| useSameSource | boolean | Indica si se utiliza la misma fuente de datos cuando otra tabla dinámica existente ya ha usado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria. |

**Returns:**
int - El índice de caché añadido.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Agrega una nueva tabla dinámica.

**Remarks**

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de octubre de 2026. Disculpas por cualquier inconveniente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| celda | java.lang.String | La celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |
| useSameSource | boolean | Indica si se utiliza la misma fuente de datos cuando otra tabla dinámica existente ya ha usado esa fuente de datos. Si la propiedad es verdadera, ahorrará memoria cuando la misma fuente de datos se haya reunido en una única caché de tabla dinámica. |
| isXlsClassic | boolean | Indica si se agrega una tabla dinámica clásica de Excel 97-2003. |

**Returns:**
int - El índice de caché añadido.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


Agrega un nuevo objeto de tabla dinámica a la colección con múltiples rangos de consolidación como fuente de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String[] | Los rangos de consolidación múltiple, como \\{"Sheet1!A1:C8","Sheet2!A1:B8"\\} |
| isAutoPage | boolean | Indica si se crea automáticamente un campo de página único. Si es verdadero, el siguiente parámetro pageFields será ignorado |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Los elementos del campo de página de la tabla dinámica. |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice del nuevo PivotTable añadido.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


Agrega un nuevo objeto de tabla dinámica a la colección con múltiples rangos de consolidación como fuente de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String[] | Los rangos de consolidación múltiple, como \\{"Sheet1!A1:C8","Sheet2!A1:B8"\\} |
| isAutoPage | boolean | Indica si se crea automáticamente un campo de página único. Si es verdadero, el siguiente parámetro pageFields será ignorado. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Los elementos del campo de página de la tabla dinámica. |
| destCellName | java.lang.String | destCellName El nombre del nuevo informe de PivotTable. |
| tableName | java.lang.String | el nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice del nuevo PivotTable añadido.
### clear() {#clear--}
```
public void clear()
```


Borra todas las tablas dinámicas.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
### dispose() {#dispose--}
```
public void dispose()
```


Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados.

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
### get(int index) {#get-int-}
```
public PivotTable get(int index)
```


Obtiene el informe de PivotTable por índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


Obtiene el [PivotTable](../../com.aspose.cells/pivottable) ubicado en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int |  |
| columna | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


Obtiene el informe de PivotTable por el nombre del PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Devuelve un enumerador que recorre la instancia de CollectionBase.

**Returns:**
java.util.Iterator - Un iterador para la instancia de CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


Elimina el PivotTable especificado y elimina los datos del PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable objeto |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


Elimina el PivotTable especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable objeto |
| keepData | boolean | Indica si se deben conservar los datos de la tabla dinámica |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el PivotTable en el índice especificado y elimina los datos del PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice de posición en la colección de PivotTable |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


Elimina el PivotTable en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice de posición en la colección de PivotTable |
| keepData | boolean | Indica si se deben conservar los datos de la tabla dinámica |

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

