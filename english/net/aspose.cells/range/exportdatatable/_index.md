---
title: Range.ExportDataTable
second_title: Aspose.Cells for .NET API Reference
description: Range method. Exports data in this range to a DataTable object
type: docs
url: /net/aspose.cells/range/exportdatatable/
---
## ExportDataTable() {#exportdatatable}

Exports data in this range to a DataTable object.

```csharp
public DataTable ExportDataTable()
```

### Return Value

Exported DataTable object.

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(ExportTableOptions) {#exportdatatable_1}

Exports data in this range to a DataTable object.

```csharp
public DataTable ExportDataTable(ExportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | ExportTableOptions | The options of exporting range to datatable. |

### Return Value

Exported DataTable object.

### Examples

```csharp
// Called: var dataTable = designer.Workbook.Worksheets.GetRangeByName(&amp;quot;Names&amp;quot;).ExportDataTable(options);
[Test]
        public void Method_ExportTableOptions_()
        {
            Workbook source = new Workbook(Constants.sourcePath + &quot;CELLSNET46252.xlsx&quot;);
            WorkbookDesigner designer = new WorkbookDesigner(source);
            var range = designer.Workbook.Worksheets.GetRangeByName(&quot;Names&quot;);
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            var dataTable = designer.Workbook.Worksheets.GetRangeByName(&quot;Names&quot;).ExportDataTable(options);
            Assert.AreEqual(2, dataTable.Rows.Count);
        }
```

### See Also

* class [ExportTableOptions](../../exporttableoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


