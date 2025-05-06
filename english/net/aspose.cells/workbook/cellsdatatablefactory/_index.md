---
title: Workbook.CellsDataTableFactory
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the factory for building ICellsDataTable from custom objects
type: docs
url: /net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Gets the factory for building ICellsDataTable from custom objects

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Examples

```csharp
// Called: cells.ImportData(wb.CellsDataTableFactory.GetInstance(al.ToArray(), true),
[Test]
        public void Property_CellsDataTableFactory()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            ArrayList al = new ArrayList();
            al.Add(&quot;1&quot;);
            al.Add(&quot;2&quot;);
            al.Add(&quot;3&quot;);
            cells.ImportArrayList(al, 0, 0, true);
            for (int i = 0; i &lt; 3; i++)
            {
                Assert.AreEqual(al[i], cells[i, 0].Value);
            }
            cells.ImportData(wb.CellsDataTableFactory.GetInstance(al.ToArray(), true),
                0, 0, new ImportTableOptions() { ConvertNumericData = true, IsFieldNameShown = false, });
            for (int i = 0; i &lt; 3; i++)
            {
                Assert.AreEqual(i + 1, cells[i, 0].IntValue, &quot;ConvertNum&quot;);
            }
        }
```

### See Also

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


