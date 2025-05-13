---
title: Style.ForegroundArgbColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets and sets the foreground color with a 32bit ARGB value
type: docs
url: /net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

Gets and sets the foreground color with a 32-bit ARGB value.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(-16384, workbook.Worksheets[0].Cells["Q8"].GetDisplayStyle().ForegroundArgbColor);
public void Style_Property_ForegroundArgbColor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    Assert.AreEqual(-16384, workbook.Worksheets[0].Cells["Q8"].GetDisplayStyle().ForegroundArgbColor);
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


