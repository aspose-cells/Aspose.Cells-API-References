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
// Called: DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 9, 7, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "SmartMarker/CellsJava43186_data.xlsx");
            DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 9, 7, true);
            dt.TableName = "products1";
            Workbook tem = new Workbook(Constants.sourcePath + "SmartMarker/CellsJava43186_template.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(tem);
            designer.RepeatFormulasWithSubtotal = true;
            designer.SetDataSource(dt);
            designer.Process();
            Assert.AreEqual("=SUM(C5:D5)", tem.Worksheets[0].Cells["E5"].Formula);
            tem.Save(Constants.destPath + "CellsJava43186.xlsx");
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
// Called: DataTable table = sheet.Cells.ExportDataTable(0, 0, maxRow, maxCol, opts);
[Test]
        public void Method_ExportTableOptions_()
        {
            Workbook excel = new Workbook(Constants.sourcePath + "CellsNet58119.xlsx");
            Worksheet sheet = excel.Worksheets[0];
            int maxRow = sheet.Cells.MaxDataRow + 1;
            int maxCol = sheet.Cells.MaxDataColumn + 1;

            var opts = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true,
                AllowDBNull = true
            };
            DataTable table = sheet.Cells.ExportDataTable(0, 0, maxRow, maxCol, opts);
            Assert.AreEqual(2, table.Columns.Count);
            Assert.AreEqual(5, table.Rows.Count);
            Assert.IsTrue(table.Columns.Contains("id"));
            Assert.AreEqual("System.Double", table.Columns["id"].DataType.FullName);
            Assert.IsTrue(table.Columns.Contains("value date"));
            Assert.AreEqual("System.DateTime", table.Columns["value date"].DataType.FullName);
        }
```

### See Also

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


