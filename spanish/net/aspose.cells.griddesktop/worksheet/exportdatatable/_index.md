---
title: "Worksheet.ExportDataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Exporta los datos de la colección Cells de un Worksheet a un objeto DataTable especificado"
type: docs
url: /es/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}

Exporta datos de la colección Cells de una Worksheet a un objeto DataTable especificado.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El número de fila de la primera celda a exportar. |
| startColumn | Int32 | El número de columna de la primera celda a exportar. |
| filas | Int32 | Número de filas a importar. |
| columnas | Int32 | Número de columnas a importar. |
| isVertical | Booleano | Verdadero si una fila en el control representa una fila en DataTable. Falso si una columna en el control representa una fila en DataTable. |

### Valor de retorno

Objeto DataTable exportado.

### Observaciones

El método permite crear primero un objeto DataTable. Luego exporta datos al objeto DataTable. Si dataTable no está configurado como válido, el método devolverá un nuevo objeto DataTable llamando al método sobrecargado 'Export(bool exportColumnName, bool isVertical)'.

### Ejemplos

```csharp
[C#]

DataTable dataTable = new DataTable();
dataTable.Columns.Add("Column a",System.Type.GetType("System.String"));
dataTable.Columns.Add("Column b");
dataTable.Columns.Add("Column c");
dataTable.Columns.Add("Column d",System.Type.GetType("System.Double"));
dataTable.Columns.Add("Column e",System.Type.GetType("System.Int32"));
dataTable.Columns.Add("Column f",System.Type.GetType("System.Int32"));
DataTable exportTable = gridDesktop.Worksheets[0].Export(dataTable,1,0,10,6,true);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim dataTable As DataTable =  New DataTable() 
dataTable.Columns.Add("Column a",System.Type.GetType("System.String"))
dataTable.Columns.Add("Column b")
dataTable.Columns.Add("Column c")
dataTable.Columns.Add("Column d",System.Type.GetType("System.Double"))
dataTable.Columns.Add("Column e",System.Type.GetType("System.Int32"))
dataTable.Columns.Add("Column f",System.Type.GetType("System.Int32"))
Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(dataTable,1,0,10,6,True) 
DataGrid1.SetDataBinding(exportTable)
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}

Exporta datos de la colección Cells de una Worksheet a un nuevo objeto DataTable.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El número de fila de la primera celda a exportar. |
| startColumn | Int32 | El número de columna de la primera celda a exportar. |
| filas | Int32 | Número de filas a importar. |
| columnas | Int32 | Número de columnas a importar. |
| exportColumnName | Booleano | Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. |
| isVertical | Booleano | Verdadero si una fila en el control representa una fila en DataTable. Falso si una columna en el control representa una fila en DataTable. |

### Valor de retorno

Objeto DataTable exportado.

### Ejemplos

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}

Exporta datos de la colección [`Cells`](../cells/) a un objeto DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    GridExportTableOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de fila de la primera celda a exportar. |
| firstColumn | Int32 | El número de columna de la primera celda a exportar. |
| totalRows | Int32 | Número de filas a importar. |
| totalColumns | Int32 | Número de columnas a importar. |
| opciones | GridExportTableOptions | Todas las opciones de exportación de tabla |

### Valor de retorno

Objeto DataTable exportado.

### Ver también

* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


