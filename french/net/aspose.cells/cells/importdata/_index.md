---
title: ImportData
second_title: Référence de l'API Aspose.Cells pour .NET
description: Importe des données à partir dunIDataReader objet.
type: docs
weight: 980
url: /fr/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importe des données à partir d'unIDataReader objet.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| reader | IDataReader | LaIDataReader objet qui contient des données. |
| firstRow | Int32 | Le numéro de ligne de la première cellule à importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule à importer. |

### Return_Value

Nombre total de lignes importées.

### Voir également

* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importe des données à partir d'unIDataReader objet.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| reader | IDataReader | LaIDataReader objet qui contient des données. |
| firstRow | Int32 | Le numéro de ligne de la première cellule à importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule à importer. |
| options | ImportTableOptions | Les options d'importation de table. |

### Return_Value

Nombre total de lignes importées.

### Voir également

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importer des données à partir d'un tableau de données personnalisé.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| table | ICellsDataTable | La table de données personnalisée. |
| firstRow | Int32 | Index de la première ligne. |
| firstColumn | Int32 | Index de la première colonne. |
| options | ImportTableOptions | Les options d'importation |

### Voir également

* interface [ICellsDataTable](../../icellsdatatable)
* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importer des données à partir d'un tableau de données personnalisé.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| table | DataTable | LaDataTable objet à importer. |
| firstRow | Int32 | Index de la première ligne. |
| firstColumn | Int32 | Index de la première colonne. |
| options | ImportTableOptions | Les options d'importation |

### Return_Value

Nombre total de lignes importées.

### Exemples

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Importer des données
DataTable dt = new DataTable("Products");
dt.Columns.Add("Product_ID",typeof(Int32));
dt.Columns.Add("Product_Name",typeof(string));
dt.Columns.Add("Units_In_Stock",typeof(Int32));
DataRow dr = dt.NewRow();
dr[0] = 1;
dr[1] = "Aniseed Syrup";
dr[2] = 15;
dt.Rows.Add(dr);
dr = dt.NewRow();
dr[0] = 2;
dr[1] = "Boston Crab Meat";
dr[2] = 123;
dt.Rows.Add(dr);
ImportTableOptions options = new ImportTableOptions();
options.IsFieldNameShown = true;
cells.ImportData(dt, 12, 12, options);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Importer des données
Dim dt as DataTable = new DataTable("Employee")
dt.Columns.Add("Employee_ID",typeof(Int32))
dt.Columns.Add("Employee_Name",typeof(string))
dt.Columns.Add("Gender",typeof(string))
Dim dr as DataRow = dt.NewRow()
dr(0) = 1
dr(1) = "John Smith"
dr(2) = "Male"
dt.Rows.Add(dr)
dr = dt.NewRow()
dr(0) = 2
dr(1) = "Mary Miller"
dr(2) = "Female"
dt.Rows.Add(dr)
Dim options as ImportTableOptions = new ImportTableOptions()
options.IsFieldNameShown = True
cells.ImportData(dt, 12, 12, options)

'Exporter des données
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Voir également

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importer des données à partir de la vue des données.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| dataView | DataView | LaDataView objet à importer. |
| firstRow | Int32 | Index de la première ligne. |
| firstColumn | Int32 | Index de la première colonne. |
| options | ImportTableOptions | Les options d'importation |

### Return_Value

Nombre total de lignes importées.

### Voir également

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
