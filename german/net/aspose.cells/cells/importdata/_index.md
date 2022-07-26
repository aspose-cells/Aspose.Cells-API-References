---
title: ImportData
second_title: Aspose.Cells für .NET-API-Referenz
description: Importiert Daten von aIDataReader Objekt.
type: docs
weight: 980
url: /de/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importiert Daten von aIDataReader Objekt.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| reader | IDataReader | DasIDataReader Objekt, das Daten enthält. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Siehe auch

* class [Cells](../../cells)
* namensraum [Aspose.Cells](../../cells)
* Montage [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importiert Daten von aIDataReader Objekt.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| reader | IDataReader | DasIDataReader Objekt, das Daten enthält. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| options | ImportTableOptions | Die Optionen zum Importieren von Tabellen. |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Siehe auch

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* namensraum [Aspose.Cells](../../cells)
* Montage [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Daten aus benutzerdefinierter Datentabelle importieren.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | ICellsDataTable | Die benutzerdefinierte Datentabelle. |
| firstRow | Int32 | Index der ersten Zeile. |
| firstColumn | Int32 | Index der ersten Spalte. |
| options | ImportTableOptions | Die Importoptionen |

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable)
* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* namensraum [Aspose.Cells](../../cells)
* Montage [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Daten aus benutzerdefinierter Datentabelle importieren.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | DataTable | DasDataTable zu importierendes Objekt. |
| firstRow | Int32 | Index der ersten Zeile. |
| firstColumn | Int32 | Index der ersten Spalte. |
| options | ImportTableOptions | Die Importoptionen |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Beispiele

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Daten importieren
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

'Daten importieren
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

'Daten exportieren
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Siehe auch

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* namensraum [Aspose.Cells](../../cells)
* Montage [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Daten aus Datenansicht importieren.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataView | DataView | DasDataView zu importierendes Objekt. |
| firstRow | Int32 | Index der ersten Zeile. |
| firstColumn | Int32 | Index der ersten Spalte. |
| options | ImportTableOptions | Die Importoptionen |

### Rückgabewert

Gesamtzahl der importierten Zeilen.

### Siehe auch

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* namensraum [Aspose.Cells](../../cells)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
