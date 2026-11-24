---
title: "Worksheet.ExportDataTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Exportiert Daten aus der Cells-Sammlung eines Worksheets in ein angegebenes DataTable-Objekt"
type: docs
url: /de/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}

Exportiert Daten aus der Cells‑Sammlung eines Arbeitsblatts in ein angegebenes DataTable‑Objekt.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Zeilennummer der ersten zu exportierenden Zelle. |
| startColumn | Int32 | Die Spaltennummer der ersten zu exportierenden Zelle. |
| Zeilen | Int32 | Anzahl der zu importierenden Zeilen. |
| Spalten | Int32 | Anzahl der zu importierenden Spalten. |
| isVertical | Boolean | True, wenn eine Zeile in der Steuerung eine Zeile im DataTable darstellt. False, wenn eine Spalte in der Steuerung eine Zeile im DataTable darstellt. |

### Rückgabewert

Exportiertes DataTable-Objekt.

### Hinweise

Die Methode ermöglicht zunächst das Erstellen eines DataTable-Objekts. Anschließend werden Daten in das DataTable-Objekt exportiert. Wenn das DataTable nicht gültig gesetzt ist, gibt die Methode ein neues DataTable-Objekt zurück, indem sie die überladene Methode 'Export(bool exportColumnName, bool isVertical)' aufruft.

### Beispiele

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

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}

Exportiert Daten aus der Cells‑Sammlung eines Arbeitsblatts in ein neues DataTable‑Objekt.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Zeilennummer der ersten zu exportierenden Zelle. |
| startColumn | Int32 | Die Spaltennummer der ersten zu exportierenden Zelle. |
| Zeilen | Int32 | Anzahl der zu importierenden Zeilen. |
| Spalten | Int32 | Anzahl der zu importierenden Spalten. |
| exportColumnName | Boolean | Gibt an, ob die Daten in der ersten Zeile zum Spaltennamen der DataTable exportiert werden. |
| isVertical | Boolean | True, wenn eine Zeile in der Steuerung eine Zeile im DataTable darstellt. False, wenn eine Spalte in der Steuerung eine Zeile im DataTable darstellt. |

### Rückgabewert

Exportiertes DataTable-Objekt.

### Beispiele

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}

Exportiert Daten aus der [`Cells`](../cells/) Sammlung in ein DataTable-Objekt.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    GridExportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | Int32 | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | Int32 | Anzahl der zu importierenden Zeilen. |
| totalColumns | Int32 | Anzahl der zu importierenden Spalten. |
| Optionen | GridExportTableOptions | Alle Export-Tabellenoptionen |

### Rückgabewert

Exportiertes DataTable-Objekt.

### Siehe auch

* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


