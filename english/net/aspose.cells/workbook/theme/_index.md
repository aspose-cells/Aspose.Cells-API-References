---
title: Workbook.Theme
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the theme name
type: docs
url: /net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

Gets the theme name.

```csharp
public string Theme { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Theme, "Office");
public void Workbook_Property_Theme()
{
    Workbook workbook = new Workbook();
    Assert.AreEqual(workbook.Theme, "Office");
    workbook.SetThemeColor(ThemeColorType.Accent1, Color.Black);
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


