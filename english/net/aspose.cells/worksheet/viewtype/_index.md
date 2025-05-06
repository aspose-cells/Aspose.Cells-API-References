---
title: Worksheet.ViewType
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets and sets the view type
type: docs
url: /net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Gets and sets the view type.

```csharp
public ViewType ViewType { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].ViewType = ViewType.PageBreakPreview;
[Test]
        public void Property_ViewType()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].ViewType = ViewType.PageBreakPreview;
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42220.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA42220.xlsb&quot;);
            Assert.AreEqual( workbook.Worksheets[0].ViewType , ViewType.PageBreakPreview);
                
        }
```

### See Also

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


