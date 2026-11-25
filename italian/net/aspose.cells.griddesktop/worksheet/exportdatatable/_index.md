---
title: "Worksheet.ExportDataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet metodo. Esporta i dati nella collezione Cells di un Worksheet in un oggetto DataTable specificato"
type: docs
url: /it/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}

Esporta i dati nella raccolta Cells di un Worksheet in un oggetto DataTable specificato.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Il numero di riga della prima cella da esportare. |
| startColumn | Int32 | Il numero di colonna della prima cella da esportare. |
| righe | Int32 | Numero di righe da importare. |
| colonne | Int32 | Numero di colonne da importare. |
| isVertical | Booleano | Vero se una riga nel controllo rappresenta una riga in DataTable. Falso se una colonna nel controllo rappresenta una riga in DataTable. |

### Valore di ritorno

Oggetto DataTable esportato.

### Osservazioni

Il metodo consente prima di creare un oggetto DataTable. Poi esporta i dati nell'oggetto DataTable. Se dataTable non è impostato correttamente, il metodo restituirà un nuovo oggetto DataTable chiamando il metodo sovraccarico 'Export(bool exportColumnName, bool isVertical)'.

### Esempi

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

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}

Esporta i dati nella raccolta Cells di un Worksheet in un nuovo oggetto DataTable.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Il numero di riga della prima cella da esportare. |
| startColumn | Int32 | Il numero di colonna della prima cella da esportare. |
| righe | Int32 | Numero di righe da importare. |
| colonne | Int32 | Numero di colonne da importare. |
| exportColumnName | Booleano | Indica se i dati nella prima riga vengono esportati nel nome della colonna di DataTable. |
| isVertical | Booleano | Vero se una riga nel controllo rappresenta una riga in DataTable. Falso se una colonna nel controllo rappresenta una riga in DataTable. |

### Valore di ritorno

Oggetto DataTable esportato.

### Esempi

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}

Esporta i dati nella collezione [`Cells`](../cells/) in un oggetto DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    GridExportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Il numero di riga della prima cella da esportare. |
| firstColumn | Int32 | Il numero di colonna della prima cella da esportare. |
| totalRows | Int32 | Numero di righe da importare. |
| totalColumns | Int32 | Numero di colonne da importare. |
| opzioni | GridExportTableOptions | Tutte le opzioni di esportazione della tabella |

### Valore di ritorno

Oggetto DataTable esportato.

### Vedi anche

* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


