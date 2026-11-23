---
title: "Worksheet.ExportDataTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Exporte les données de la collection Cells d'une Worksheet vers un objet DataTable spécifié."
type: docs
url: /fr/net/aspose.cells.griddesktop/worksheet/exportdatatable/
---
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_1}

Exporte les données de la collection Cells d'une Worksheet vers un objet DataTable spécifié.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| startColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| lignes | Int32 | Nombre de lignes à importer. |
| colonnes | Int32 | Nombre de colonnes à importer. |
| isVertical | Boolean | Vrai si une ligne du contrôle représente une ligne du DataTable. Faux si une colonne du contrôle représente une ligne du DataTable. |

### Valeur de retour

Objet DataTable exporté.

### Remarques

La méthode permet d'abord de créer un objet DataTable. Ensuite, elle exporte les données vers l'objet DataTable. Si dataTable n'est pas valide, la méthode renverra un nouvel objet DataTable en appelant la méthode surchargée 'Export(bool exportColumnName, bool isVertical)'.

### Exemples

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

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, bool, bool) {#exportdatatable_2}

Exporte les données de la collection Cells d'une Worksheet vers un nouvel objet DataTable.

```csharp
public DataTable ExportDataTable(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| startColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| lignes | Int32 | Nombre de lignes à importer. |
| colonnes | Int32 | Nombre de colonnes à importer. |
| exportColumnName | Boolean | Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. |
| isVertical | Boolean | Vrai si une ligne du contrôle représente une ligne du DataTable. Faux si une colonne du contrôle représente une ligne du DataTable. |

### Valeur de retour

Objet DataTable exporté.

### Exemples

```csharp
[C#]

DataTable exportTable = gridDesktop.Worksheets[0].Export(0,0,10,2,true,false);
DataGrid1.SetDataBinding(exportTable, null);

[VB]

Dim exportTable As DataTable =  GridDesktop.Worksheets(0).Export(0,0,10,2,True,False) 
DataGrid1.SetDataBinding(exportTable)
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportDataTable(int, int, int, int, GridExportTableOptions) {#exportdatatable}

Exporte les données de la collection [`Cells`](../cells/) vers un objet DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    GridExportTableOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| totalRows | Int32 | Nombre de lignes à importer. |
| totalColumns | Int32 | Nombre de colonnes à importer. |
| options | GridExportTableOptions | Toutes les options d'exportation de tableau |

### Valeur de retour

Objet DataTable exporté.

### Voir aussi

* class [GridExportTableOptions](../../../aspose.cells.griddesktop.data/gridexporttableoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


