---
title: ImportData
second_title: Aspose.Cells för .NET API-referens
description: Importerar data från enIDataReader objekt.
type: docs
weight: 980
url: /sv/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importerar data från enIDataReader objekt.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| reader | IDataReader | DeIDataReader objekt som innehåller data. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |

### Returvärde

Totalt antal importerade rader.

### Se även

* class [Cells](../../cells)
* namnutrymme [Aspose.Cells](../../cells)
* hopsättning [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importerar data från enIDataReader objekt.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| reader | IDataReader | DeIDataReader objekt som innehåller data. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| options | ImportTableOptions | Alternativen för att importera tabell. |

### Returvärde

Totalt antal importerade rader.

### Se även

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* namnutrymme [Aspose.Cells](../../cells)
* hopsättning [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importera data från anpassad datatabell.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | ICellsDataTable | Den anpassade datatabellen. |
| firstRow | Int32 | Första radens index. |
| firstColumn | Int32 | Första kolumnindex. |
| options | ImportTableOptions | Importalternativen |

### Se även

* interface [ICellsDataTable](../../icellsdatatable)
* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* namnutrymme [Aspose.Cells](../../cells)
* hopsättning [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importera data från anpassad datatabell.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | DataTable | DeDataTable objekt som ska importeras. |
| firstRow | Int32 | Första radens index. |
| firstColumn | Int32 | Första kolumnindex. |
| options | ImportTableOptions | Importalternativen |

### Returvärde

Totalt antal importerade rader.

### Exempel

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Importera data
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

'Importera data
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

'Exportera data
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Se även

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* namnutrymme [Aspose.Cells](../../cells)
* hopsättning [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importera data från datavyn.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataView | DataView | DeDataView objekt som ska importeras. |
| firstRow | Int32 | Första radens index. |
| firstColumn | Int32 | Första kolumnindex. |
| options | ImportTableOptions | Importalternativen |

### Returvärde

Totalt antal importerade rader.

### Se även

* class [ImportTableOptions](../../importtableoptions)
* class [Cells](../../cells)
* namnutrymme [Aspose.Cells](../../cells)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
