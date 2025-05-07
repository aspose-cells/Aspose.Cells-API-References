---
title: Font.Underline
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the font underline type
type: docs
url: /net/aspose.cells/font/underline/
---
## Font.Underline property

Gets or sets the font underline type.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells["B6"].GetStyle().Font.Underline, FontUnderlineType.Single);
[Test]
        public void Property_Underline()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestUnderline.xlsx");
            Assert.AreEqual(workbook.Worksheets[0].Cells["B6"].GetStyle().Font.Underline, FontUnderlineType.Single);
            
        }
```

### See Also

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


