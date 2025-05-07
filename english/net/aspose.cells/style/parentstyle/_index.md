---
title: Style.ParentStyle
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets the parent style of this style
type: docs
url: /net/aspose.cells/style/parentstyle/
---
## Style.ParentStyle property

Gets the parent style of this style.

```csharp
public Style ParentStyle { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(wrongStyle.ParentStyle != null, true);
[Test]
        public void Property_ParentStyle()
        {
            Workbook main = new Workbook(Constants.sourcePath + "CELLSNET-42276.xlsm");
            Workbook workbook = new Workbook();
            workbook.Copy(main); // make a copy of original template
            Style correctStyle = main.Worksheets[0].Cells["T1"].GetStyle();
            Assert.AreEqual(correctStyle.ParentStyle != null, true);

            Style wrongStyle = workbook.Worksheets[0].Cells["T1"].GetStyle();
            Assert.AreEqual(wrongStyle.ParentStyle != null, true);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


