---
title: "WorkbookDesigner"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa una hoja de cálculo de diseñador."
type: docs
url: /es/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

Encapsula el objeto que representa una hoja de cálculo de diseñador.

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | Inicializa una nueva instancia de la clase [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | Inicializa una nueva instancia de la clase [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
## Métodos

| Método | Descripción |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | Borra todas las fuentes de datos. |
| [containsVariables()](#containsVariables--) | Indica si la primera hoja de cálculo contiene variables personalizadas. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | Indica si las fórmulas deben ser calculadas. |
| [getCallBack()](#getCallBack--) | Obtiene la interfaz de devolución de llamada del procesamiento de smartmarker. |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | Indica si el encabezado/pie de página contiene marcadores inteligentes y debe procesarse junto. |
| [getLineByLine()](#getLineByLine--) | Indica si el procesamiento del marcador inteligente se realiza línea por línea. |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | Indica si se repiten fórmulas con fila de subtotal. |
| [getSmartMarkers()](#getSmartMarkers--) | Devuelve una colección de marcadores inteligentes en una hoja de cálculo. |
| [getSortDataSource()](#getSortDataSource--) | Indica si se ordena la fuente de datos. |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | Si es TRUE, se insertará Null si el valor es ""; |
| [getUpdateReference()](#getUpdateReference--) | Indica si las referencias en otras hojas de cálculo se actualizarán. |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | Obtiene el nombre de la hoja de cálculo que contiene el marcador inteligente de variables. |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto [getWorkbook()](../../com.aspose.cells/workbookdesigner\\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos. |
| [process(boolean isPreserved)](#process-boolean-) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos. |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos. |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indica si las fórmulas deben ser calculadas. |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | Establece la interfaz de devolución de llamada del procesamiento de smartmarker. |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | Indica si la primera hoja de cálculo contiene variables personalizadas. |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | Establece la fuente de datos de un objeto [ICellsDataTable](../../com.aspose.cells/icellsdatatable). |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | Establece la vinculación de datos a una variable. |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | Establece la fuente de datos. |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | Establece la fuente de datos. |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | Establece la fuente de datos. |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | Indica si el encabezado/pie de página contiene marcadores inteligentes y debe procesarse junto. |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | Establece el valor de cadena JSON como fuente de datos de los marcadores inteligentes. |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | Indica si el procesamiento del marcador inteligente se realiza línea por línea. |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | Indica si se repiten fórmulas con fila de subtotal. |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | Indica si se ordena la fuente de datos. |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | Si es TRUE, se insertará Null si el valor es ""; |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indica si las referencias en otras hojas de cálculo se actualizarán. |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | Establece el nombre de la hoja de cálculo que contiene el marcador inteligente de variables. |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | Establece el objeto [getWorkbook()](../../com.aspose.cells/workbookdesigner\\#getWorkbook--). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


Inicializa una nueva instancia de la clase [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


Inicializa una nueva instancia de la clase [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | El archivo de libro de trabajo de plantilla. |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


Borra todas las fuentes de datos.

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


Indica si la primera hoja de cálculo contiene variables personalizadas.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad WorkbookDesigner.VariablesWorksheetName, en su lugar. Esta propiedad será eliminada 3 meses después, a partir de septiembre de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
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
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indica si las fórmulas deben ser calculadas.

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


Obtiene la interfaz de devolución de llamada del procesamiento de smartmarker.

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


Indica si el encabezado/pie de página contiene marcadores inteligentes y debe procesarse junto.

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


Indica si el procesamiento del marcador inteligente se realiza línea por línea.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice marcadores inteligentes de rango. Esta propiedad será eliminada 12 meses después, a partir de julio de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


Indica si se repiten fórmulas con fila de subtotal.

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


Devuelve una colección de marcadores inteligentes en una hoja de cálculo.

**Remarks**

Se crea una matriz de cadenas en cada llamada. La matriz se ordena y se eliminan los valores duplicados.

**Returns:**
java.lang.String[] - Una colección de marcadores inteligentes
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


Indica si se ordena la fuente de datos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado. La fuente de datos JSON se ordenará si el marcador inteligente contiene parámetros ascendente y descendente.

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


Si es TRUE, se insertará Null si el valor es "";

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Indica si las referencias en otras hojas de cálculo se actualizarán.

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


Obtiene el nombre de la hoja de cálculo que contiene el marcador inteligente de variables.

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtiene el objeto [getWorkbook()](../../com.aspose.cells/workbookdesigner\\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
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




### process() {#process--}
```
public void process()
```


Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isPreserved | boolean | True si el marcador inteligente no reconocido se conserva. |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice marcadores inteligentes de rango. Esta propiedad será eliminada 12 meses después, a partir de julio de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | El rango a procesar |
| isPreserved | boolean | True si el marcador inteligente no reconocido se conserva. |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.

**Remarks**

Este método funciona a nivel de hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | Índice de hoja de cálculo. |
| isPreserved | boolean | True si el marcador inteligente no reconocido se conserva. |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indica si las fórmulas deben ser calculadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


Establece la interfaz de devolución de llamada del procesamiento de smartmarker.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


Indica si la primera hoja de cálculo contiene variables personalizadas.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad WorkbookDesigner.VariablesWorksheetName, en su lugar. Esta propiedad será eliminada 3 meses después, a partir de septiembre de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


Establece la fuente de datos de un objeto [ICellsDataTable](../../com.aspose.cells/icellsdatatable).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataSource | java.lang.String | El nombre de la fuente de datos. |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | tabla de datos. |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


Establece la vinculación de datos a una variable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| variable | java.lang.String | Nombre de variable creado usando marcador inteligente. |
| datos | java.lang.Object | Datos de origen. |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


Establece la fuente de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataSource | java.lang.String | El nombre de la fuente de datos. |
| rs | java.sql.ResultSet | El conjunto de resultados. |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


Establece la fuente de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataSource | java.lang.String | El nombre de la fuente de datos. |
| rs | java.sql.ResultSet | El conjunto de resultados. |
| rowCount | int | El recuento de datos del conjunto de resultados dado. Debe ser el recuento exacto de filas o -1; si el conjunto de resultados es solo de avance, el usuario debe proporcionar el recuento exacto de filas aquí, de lo contrario el marcador inteligente puede no procesarse correctamente cuando la propiedad "noadd" del marcador inteligente no está establecida. |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


Establece la fuente de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rs | java.sql.ResultSet | El conjunto de resultados. |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


Indica si el encabezado/pie de página contiene marcadores inteligentes y debe procesarse junto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


Establece el valor de cadena JSON como fuente de datos de los marcadores inteligentes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la tabla. Si el valor de JSON representa un objeto, puede ser nulo. |
| json | java.lang.String | El valor de la cadena Json. |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


Indica si el procesamiento del marcador inteligente se realiza línea por línea.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice marcadores inteligentes de rango. Esta propiedad será eliminada 12 meses después, a partir de julio de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


Indica si se repiten fórmulas con fila de subtotal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


Indica si se ordena la fuente de datos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado. La fuente de datos JSON se ordenará si el marcador inteligente contiene parámetros ascendente y descendente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


Si es TRUE, se insertará Null si el valor es "";

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Indica si las referencias en otras hojas de cálculo se actualizarán.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


Establece el nombre de la hoja de cálculo que contiene el marcador inteligente de variables.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


Establece el objeto [getWorkbook()](../../com.aspose.cells/workbookdesigner\\#getWorkbook--).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

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

