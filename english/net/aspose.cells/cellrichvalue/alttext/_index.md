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
// Called: Assert.AreEqual("test alt text", c4.GetRichValue().AltText);
[Test]
        public void Property_AltText()
        { 
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA46150.xlsx");
            Cell c4 = workbook.Worksheets[0].Cells["C4"];
            Assert.AreEqual("test alt text", c4.GetRichValue().AltText);


        }
```

### See Also

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


