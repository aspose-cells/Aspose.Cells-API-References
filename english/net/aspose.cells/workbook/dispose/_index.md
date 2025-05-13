---
title: Workbook.Dispose
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Performs applicationdefined tasks associated with freeing releasing or resetting unmanaged resources
type: docs
url: /net/aspose.cells/workbook/dispose/
---
## Workbook.Dispose method

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

```csharp
public void Dispose()
```

### Examples

```csharp
// Called: wb.Dispose();
private void Workbook_Method_Dispose(Stream s, int startRow, int startColumn, int endRow, int endColumn,
            string sheetName, Workbook wbBase, string info)
        {
            LoadOptions opts = new LoadOptions();
            LightCellsDataHandlerVisitCells v = new LightCellsDataHandlerVisitCells(info,
                wbBase, startRow, startColumn, endRow, endColumn, sheetName);
            opts.LightCellsDataHandler = v;
            Workbook wb = new Workbook(s, opts);
            string err = v.GetError();
            wb.Dispose();
            if (err != null)
            {
                Assert.Fail(info + ":\n" + err);
            }
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


