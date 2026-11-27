---
title: "Worksheet.ExportDataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Exporterar data i Cells-samlingen i ett Worksheet till ett specificerat DataTable-objekt"
type: docs
url: /sv/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}

Exporterar data i Cells-samlingen i ett Worksheet till ett specificerat DataTable-objekt.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| rader | Int32 | Antal rader att importera. |
| kolumner | Int32 | Antal kolumner att importera. |
| ärVertikal | Boolean | Sant om en rad i kontrollen representerar en rad i DataTable. Falskt om en kolumn i kontrollen representerar en rad i DataTable. |

### Returvärde

Exporterad DataTable‑objekt.

### Anmärkningar

Metoden tillåter först att skapa ett DataTable-objekt. Därefter exporteras data till DataTable-objektet. Om dataTable inte är giltigt inställt, kommer metoden att returnera ett nytt DataTable-objekt genom att anropa överlagrad metod 'Export(bool exportColumnName, bool isVertical)'.

### Exempel

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

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}

Exporterar data i Cells-samlingen i ett Worksheet till ett nytt DataTable-objekt.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| rader | Int32 | Antal rader att importera. |
| kolumner | Int32 | Antal kolumner att importera. |
| exportColumnName | Boolean | Anger om data i den första raden exporteras till kolumnnamnet i DataTable. |
| ärVertikal | Boolean | Sant om en rad i kontrollen representerar en rad i DataTable. Falskt om en kolumn i kontrollen representerar en rad i DataTable. |

### Returvärde

Exporterad DataTable‑objekt.

### Exempel

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}

Exporterar data i [`Cells`](../cells/) samlingen till ett DataTable-objekt.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    GridExportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| firstColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | Int32 | Antal rader att importera. |
| totalColumns | Int32 | Antal kolumner att importera. |
| alternativ | GridExportTableOptions | Alla exporttabellalternativ |

### Returvärde

Exporterad DataTable‑objekt.

### Se även

* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


