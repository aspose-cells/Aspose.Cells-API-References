---
title: ImportTableOptions.ShiftFirstRowDown
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether shifting the first row down when inserting rows
type: docs
url: /net/aspose.cells/importtableoptions/shiftfirstrowdown/
---
## ImportTableOptions.ShiftFirstRowDown property

Indicates whether shifting the first row down when inserting rows.

```csharp
public bool ShiftFirstRowDown { get; set; }
```

### Examples

```csharp
// Called: ShiftFirstRowDown = false,
[Test]
        public void Property_ShiftFirstRowDown()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;insertDelete/N55086.xlsx&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            DataTable table = new DataTable();
            table.Columns.Add(new DataColumn());
            table.Columns.Add(new DataColumn());
            table.Rows.Add(&quot;A&quot;, &quot;&quot;);
            table.Rows.Add(null, null);
            table.Rows.Add(&quot;A&quot;, &quot;A&quot;);

            var importTableOptions = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = false,
                InsertRows = true,
            };
            cells.ImportData(table, 3, 0, importTableOptions);
            Assert.AreEqual(&quot;=IF(AND(A3&lt;&gt;\&quot;X\&quot;,A4=B4),\&quot;Yes\&quot;,\&quot;no\&quot;)&quot;, cells[3, 3].Formula, &quot;D4.Formula&quot;);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


