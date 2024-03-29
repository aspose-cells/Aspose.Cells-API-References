---
title: ExportDataTable
second_title: Aspose.Cells för .NET API-referens
description: Exporterar data i cellsamlingen i ett kalkylblad till ett specificerat DataTable-objekt.
type: docs
weight: 650
url: /sv/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(DataTable, int, int, int, int, bool) {#exportdatatable_1}

Exporterar data i cellsamlingen i ett kalkylblad till ett specificerat DataTable-objekt.

```csharp
public DataTable ExportDataTable(DataTable dataTable, int startRow, int startColumn, int rows, 
    int columns, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataTable | DataTable | DataTable-objektet som exporterar data till. |
| startRow | Int32 | Radnumret för den första cellen som ska exporteras ut. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras ut. |
| rows | Int32 | Antal rader som ska importeras. |
| columns | Int32 | Antal kolumner som ska importeras. |
| isVertical | Boolean | Sant om en rad i kontrollen representerar en rad i DataTable. Falskt om en kolumn i kontrollen representerar en rad i DataTable. |

### Returvärde

Exporterat DataTable-objekt.

### Anmärkningar

Metoden tillåter först att skapa ett DataTable-objekt. Exporterar sedan data till DataTable-objektet. Om dataTable inte är giltigt kommer metoden att returnera ett nytt DataTable-objekt genom att anropa överbelastningsmetoden 'Export(bool exportColumnName, bool isVertical)'.

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

* class [Worksheet](../../worksheet)
* namnutrymme [Aspose.Cells.GridDesktop](../../worksheet)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable}

Exporterar data i cellsamlingen i ett kalkylblad till ett nytt DataTable-objekt.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska exporteras ut. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras ut. |
| rows | Int32 | Antal rader som ska importeras. |
| columns | Int32 | Antal kolumner som ska importeras. |
| exportColumnName | Boolean | Anger om data i den första raden exporteras till datatabellens kolumnnamn. |
| isVertical | Boolean | Sant om en rad i kontrollen representerar en rad i DataTable. Falskt om en kolumn i kontrollen representerar en rad i DataTable. |

### Returvärde

Exporterat DataTable-objekt.

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

* class [Worksheet](../../worksheet)
* namnutrymme [Aspose.Cells.GridDesktop](../../worksheet)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
