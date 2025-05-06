---
title: CellArea.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the end column of this area
type: docs
url: /net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Gets or set the end column of this area.

```csharp
public int EndColumn;
```

### Examples

```csharp
// Called: Assert.AreEqual(fcs.GetCellArea(0).EndColumn,4);
[Test]
        public void Field_EndColumn()
        {
            var wbd = new WorkbookDesigner();
            wbd.Workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/CELLSNET46048.xlsx&quot;);

            wbd.SetDataSource(&quot;Array1&quot;, new string[5] { &quot;A&quot;, &quot;B&quot;, &quot;C&quot;, &quot;D&quot;, &quot;E&quot; });

            var dataTable = new DataTable(&quot;Table1&quot;);
            dataTable.Columns.Add(&quot;ColumnA&quot;);

            for (var i = 0; i &lt; 5; i++)
            {
                var dr = dataTable.NewRow();
                dr[&quot;ColumnA&quot;] = &quot;Row&quot; + i;
                dataTable.Rows.Add(dr);
            }

            wbd.SetDataSource(dataTable);

            wbd.Process();
            FormatConditionCollection fcs = wbd.Workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs.GetCellArea(0).EndColumn,4);
            wbd.Workbook.Save(Constants.destPath + &quot;CELLSNET46048.xlsx&quot;);
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


