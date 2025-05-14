---
title: WorkbookRender.PageCount
second_title: Aspose.Cells for .NET API Reference
description: WorkbookRender property. Gets the total page count of workbook
type: docs
url: /net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

Gets the total page count of workbook.

```csharp
public int PageCount { get; }
```

### Examples

```csharp
// Called: for (int i = 0; i < wr.PageCount; i++)
private void WorkbookRender_Property_PageCount(Workbook wb, string fnId)
        {
            WorkbookRender wr = new WorkbookRender(wb, new ImageOrPrintOptions()
            { OnePagePerSheet = true });
            for (int i = 0; i < wr.PageCount; i++)
            {
                wr.ToImage(i, Constants.checkPath + "License/PluginImage"
                    + fnId + "_" + i + ".png");
            }
        }
```

### See Also

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


