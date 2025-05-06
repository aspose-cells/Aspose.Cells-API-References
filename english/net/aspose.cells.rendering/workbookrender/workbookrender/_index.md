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
// Called: WorkbookRender wr = new WorkbookRender(wb, imgOpt);
[Test]
        public void WorkbookRender_Constructor() 
        {
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.PrintingPage = PrintingPageType.IgnoreBlank;

            {
                Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45252/log_scale_test_1-_crashes_system.xlsx&quot;);
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(4, wr.PageCount);
            }

            {
                Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45252/Chart.xlsx&quot;);
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(2, wr.PageCount);
            }

            {
                Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45252/Calibri2.xlsx&quot;);
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(3, wr.PageCount);
            }
        }
```

### See Also

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


