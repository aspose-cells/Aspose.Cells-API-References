---
title: Style.IsNumberFormatApplied
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicate whether the number formatting should be applied
type: docs
url: /net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

Indicate whether the number formatting should be applied.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### Remarks

Only for named style.

### Examples

```csharp
// Called: Assert.IsTrue(style.IsNumberFormatApplied);
[Test]
        public void Property_IsNumberFormatApplied()
        {
            Workbook asposeWorkbook;
            LoadOptions options = new LoadOptions();
            asposeWorkbook = new Workbook(Constants.sourcePath + "CELLSJAVA45750.xlsx", options);
            Style style = asposeWorkbook.GetNamedStyle("TestStyle");
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


