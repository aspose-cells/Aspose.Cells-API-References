---
title: Interface ICellsDataTable
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ICellsDataTable interface. Represents data table
type: docs
url: /net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Represents data table.

```csharp
public interface ICellsDataTable
```

## Properties

| Name | Description |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Gets the columns' name. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Gets the count of the records. -1 for unknown records count. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Gets the data stored in the column specified by index. (2 indexers) |

## Methods

| Name | Description |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Move the cursor to the front of this object, just before the first row. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Moves the cursor down one row from its current position. |

### Examples

```csharp
// Called: ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
[Test]
        public void Type_ICellsDataTable()
        {
            Workbook wb = new Workbook();

            ArrayList dataLists = new ArrayList();
            dataLists.Add(new object[] { &quot;Name&quot;, &quot;Age&quot;, &quot;Gender&quot; });
            dataLists.Add(new object[] { &quot;Alice&quot;, 30, &quot;Female&quot; });
            dataLists.Add(new object[] { &quot;Bob&quot;, 25, &quot;Male&quot; });
            dataLists.Add(new object[] { &quot;Charlie&quot;, 35, &quot;Male&quot; });

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);

            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Assert.AreEqual(&quot;Alice&quot;, wb.Worksheets[0].Cells[&quot;A2&quot;].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
            Assert.AreEqual(&quot;Bob&quot;, wb.Worksheets[1].Cells[&quot;A3&quot;].StringValue);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


