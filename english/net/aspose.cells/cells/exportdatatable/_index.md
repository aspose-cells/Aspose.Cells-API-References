---
title: Cells.ExportDataTable
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Exports data in the Cells collection to a DataTable object
type: docs
url: /net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

Exports data in the [`Cells`](../) collection to a DataTable object.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |

### Return Value

Exported DataTable object.

### Remarks

If you use this method to export a block of data, please be sure that the data in a column should be the same data type. Otherwise, use the [`ExportDataTableAsString`](../exportdatatableasstring/) method instead.

### Examples

```csharp
[C#]


string designerFile = "List.xls";
Workbook excel = new Workbook(designerFile);
Worksheet sheet = excel.Worksheets[0];
DataTable dt = sheet.Cells.ExportDataTable(6, 1, 69, 4);

[Visual Basic]


Dim designerFile As String = "List.xls"
Dim excel As excel = New excel(designerFile)
Dim sheet As Worksheet = excel.Worksheets(0)
Dim dt As DataTable = sheet.Cells.ExportDataTable(6, 1, 69, 4)
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

Exports data in the [`Cells`](../) collection to a DataTable object.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
| exportColumnName | Boolean | Indicates whether the data in the first row are exported to the column name of the DataTable. |

### Return Value

Exported DataTable object.

### Examples

```csharp
// Called: DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 11, 5, true);
public void Cells_Method_ExportDataTable()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 11, 5, true);
    WorkbookDesigner d = new WorkbookDesigner();
    d.Workbook = workbook;
    dt.TableName = "Report";
    d.SetDataSource(dt);
    d.Process();
    workbook.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

Exports data in the [`Cells`](../) collection to a DataTable object.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
| options | ExportTableOptions | All export table options |

### Return Value

Exported DataTable object.

### Examples

```csharp
// Called: dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
public void Cells_Method_ExportDataTable()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells["A1"].PutValue(1.23356);
    Style style = cells["A1"].GetStyle();
    style.Custom = "0.00";
    cells["A1"].SetStyle(style);
    ExportTableOptions etOpt = new ExportTableOptions();
    etOpt.ExportColumnName = false;
    etOpt.ExportAsString = true;
    etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
    DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
    Assert.AreEqual(dt.Rows[0][0].ToString(), "1.23");
    etOpt.FormatStrategy = CellValueFormatStrategy.None;
    dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
    Assert.AreEqual(dt.Rows[0][0].ToString(), "1.23356");
    etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
    dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
    Assert.AreEqual(dt.Rows[0][0].ToString(), "1.23");
}
```

### See Also

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


