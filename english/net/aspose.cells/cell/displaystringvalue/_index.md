---
title: Cell.DisplayStringValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the formatted string value of this cell by cells display style
type: docs
url: /net/aspose.cells/cell/displaystringvalue/
---
## Cell.DisplayStringValue property

Gets the formatted string value of this cell by cell's display style.

```csharp
public string DisplayStringValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Dec-16", ccc.DisplayStringValue, "Formatted by Style.Number=17 for German");
[Test]
        public void Property_DisplayStringValue()
        {
            Workbook wb = new Workbook();
            Cell ccc = wb.Worksheets[0].Cells[0, 0];
            Style style = ccc.GetStyle();
            style.Number = 17;
            ccc.SetStyle(style);
            ccc.PutValue(42720);
            wb.Settings.Region = CountryCode.USA;
            Assert.AreEqual("Dec-16", ccc.DisplayStringValue, "Formatted by Style.Number=17 for German");
            wb.Settings.Region = CountryCode.Germany;
            Assert.AreEqual("Dez 16", ccc.DisplayStringValue, "Formatted by Style.Number=17 for German");
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


