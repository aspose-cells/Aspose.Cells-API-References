---
title: CellRichValue.AltText
second_title: Aspose.Cells for .NET API Reference
description: CellRichValue property. Gets the alt text associated with the image
type: docs
url: /net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

Gets the alt text associated with the image.

```csharp
public virtual string AltText { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;test alt text&amp;quot;, c4.GetRichValue().AltText);
[Test]
        public void Property_AltText()
        { 
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA46150.xlsx&quot;);
            Cell c4 = workbook.Worksheets[0].Cells[&quot;C4&quot;];
            Assert.AreEqual(&quot;test alt text&quot;, c4.GetRichValue().AltText);


        }
```

### See Also

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


