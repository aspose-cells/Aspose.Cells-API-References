---
title: Style.IsProtectionApplied
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicate whether the protection formatting should be applied
type: docs
url: /net/aspose.cells/style/isprotectionapplied/
---
## Style.IsProtectionApplied property

Indicate whether the protection formatting should be applied.

```csharp
public bool IsProtectionApplied { get; set; }
```

### Remarks

Only for named style.

### Examples

```csharp
// Called: Assert.IsFalse(style.IsProtectionApplied);
public void Style_Property_IsProtectionApplied()
{
    Workbook asposeWorkbook;
    LoadOptions options = new LoadOptions();
    asposeWorkbook = new Workbook(Constants.sourcePath + "example.xlsx", options);
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


