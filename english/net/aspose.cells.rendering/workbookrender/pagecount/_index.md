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
// Called: Assert.IsTrue(wr.PageCount &amp;gt;= 30);
[Test]
        public void Property_PageCount()
        {
            Workbook wb = new Workbook(Constants.TemplatePath + &quot;CELLSNETCORE-154.xls&quot;);

            WorkbookRender wr = new WorkbookRender(wb, new ImageOrPrintOptions());
            Assert.IsTrue(wr.PageCount &gt;= 30);
        }
```

### See Also

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


