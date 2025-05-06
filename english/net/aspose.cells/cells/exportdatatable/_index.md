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
// Called: DataTable dt = wsData.Cells.ExportDataTable(0, 0, wsData.Cells.LastCell.Row + 1, wsData.Cells.LastCell.Column + 1, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wbTemplate = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CellsNet57354_EquipPivot.xlsx&quot;);
            Workbook wbData = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CellsNet57354_Data.xlsx&quot;);

            Worksheet wsTemplate = wbTemplate.Worksheets[1];
            Worksheet wsData = wbData.Worksheets[0];

            DataTable dt = wsData.Cells.ExportDataTable(0, 0, wsData.Cells.LastCell.Row + 1, wsData.Cells.LastCell.Column + 1, true);

            ListObjectCollection objects = wsTemplate.ListObjects;
            ListObject table = objects[&quot;rptEquipPivot&quot;];



            wsTemplate.Cells.DeleteRange(table.StartRow + 1, table.StartColumn, table.EndRow, table.EndColumn, ShiftType.Up);

            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = false;
            importOptions.ShiftFirstRowDown = false;
            wsTemplate.Cells.ImportData(dt, 1, 0, importOptions);
            Assert.AreEqual(&quot;=rptEquipPivot!$A$1:$CV$282&quot;, wbTemplate.Worksheets.Names[&quot;rptEquipPivot!ExternalData_1&quot;].RefersTo);
            table.Resize(0, 0, wsTemplate.Cells.LastCell.Row, wsTemplate.Cells.LastCell.Column, true);
            Assert.AreEqual(&quot;=rptEquipPivot!$A$1:$CV$282&quot;, wbTemplate.Worksheets.Names[&quot;rptEquipPivot!ExternalData_1&quot;].RefersTo);
            //If File.Exists(outfile) Then File.Delete(outfile)
            wbTemplate.Save(Constants.destPath + &quot;CellsNet57354.xlsx&quot;);
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
            string filePath = Constants.sourcePath + &quot;CellsNet55029_OldExcel.xls&quot;;
            Workbook excel = new Workbook(filePath);
            Worksheet sheet = excel.Worksheets[0];
            int maxRow = sheet.Cells.MaxDataRow + 1;
            int maxCol = sheet.Cells.MaxDataColumn + 1;

            var opts = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true,
                AllowDBNull = false

            };
            DataTable table = sheet.Cells.ExportDataTable(0, 0, maxRow, maxCol, opts);
            int errors = CheckColTypes(table);

            // Test new Excel (xlsx).
            filePath = Constants.sourcePath + &quot;CellsNet55029_NewExcel.xlsx&quot;;

            excel = new Workbook(filePath);
            sheet = excel.Worksheets[0];
            maxRow = sheet.Cells.MaxDataRow + 1;
            maxCol = sheet.Cells.MaxDataColumn + 1;

            opts = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true,
                AllowDBNull = false
            };
            table = sheet.Cells.ExportDataTable(0, 0, maxRow, maxCol, opts);
            errors += CheckColTypes(table);

            Assert.AreEqual(0, errors);
        }
```

### See Also

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


