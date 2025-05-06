---
title: Style.IsFontApplied
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicate whether the font formatting should be applied
type: docs
url: /net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Indicate whether the font formatting should be applied.

```csharp
public bool IsFontApplied { get; set; }
```

### Remarks

Only for named style.

### Examples

```csharp
// Called: Assert.IsFalse(style.IsFontApplied);
[Test]
        public void Property_IsFontApplied()
        {
            Workbook asposeWorkbook;
            LoadOptions options = new LoadOptions();
            asposeWorkbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA45750.xlsx&quot;, options);
            Style style = asposeWorkbook.GetNamedStyle(&quot;TestStyle&quot;);
            Assert.IsTrue(style.IsNumberFormatApplied);
            Assert.IsFalse(style.IsAlignmentApplied);
            Assert.IsFalse(style.IsFontApplied);
            Assert.IsFalse(style.IsBorderApplied);
            Assert.IsFalse(style.IsFillApplied);
            Assert.IsFalse(style.IsProtectionApplied);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


