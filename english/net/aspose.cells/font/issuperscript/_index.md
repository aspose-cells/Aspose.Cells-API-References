---
title: Font.IsSuperscript
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is super script
type: docs
url: /net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Gets or sets a value indicating whether the font is super script.

```csharp
public bool IsSuperscript { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(style.Font.IsSuperscript);
[Test]
        public void Property_IsSuperscript()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42264.ods");
            Style style = workbook.Worksheets[0].Cells["A8"].GetStyle();
            Assert.IsTrue(style.Font.IsSubscript);
            Assert.IsFalse(style.Font.IsSuperscript);
            style = workbook.Worksheets[0].Cells["A9"].GetStyle();
            Assert.IsFalse(style.Font.IsSubscript);
            Assert.IsTrue(style.Font.IsSuperscript);
            workbook.Save(Constants.destPath + "CELLSJAVA42264.ods");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA42264.ods");
            style = workbook.Worksheets[0].Cells["A8"].GetStyle();
            Assert.IsTrue(style.Font.IsSubscript);
            Assert.IsFalse(style.Font.IsSuperscript);
            style = workbook.Worksheets[0].Cells["A9"].GetStyle();
            Assert.IsFalse(style.Font.IsSubscript);
            Assert.IsTrue(style.Font.IsSuperscript);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


