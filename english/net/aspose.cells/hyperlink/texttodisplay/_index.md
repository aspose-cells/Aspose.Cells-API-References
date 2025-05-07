---
title: Hyperlink.TextToDisplay
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink
type: docs
url: /net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.

```csharp
public string TextToDisplay { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Hyperlinks[0].TextToDisplay, "Google ");
[Test]
        public void Property_TextToDisplay()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet42098.xlsx");
            Assert.AreEqual(workbook.Worksheets[0].Hyperlinks[0].TextToDisplay, "Google ");
        }
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


