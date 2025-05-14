---
title: WorkbookRender.WorkbookRender
second_title: Aspose.Cells for .NET API Reference
description: WorkbookRender constructor. The construct of WorkbookRender
type: docs
url: /net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

The construct of WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | Indicate which workbook to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |

### Examples

```csharp
// Called: WorkbookRender wr = new WorkbookRender(wb, new ImageOrPrintOptions());
public void WorkbookRender_Constructor()
{
    Workbook wb = new Workbook(Constants.TemplatePath + "example.xls");

    WorkbookRender wr = new WorkbookRender(wb, new ImageOrPrintOptions());
    Assert.IsTrue(wr.PageCount >= 30);
}
```

### See Also

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


