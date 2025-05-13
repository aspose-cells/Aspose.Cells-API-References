---
title: LoadOptions.IgnoreUselessShapes
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Indicates whether ignoring useless shapes
type: docs
url: /net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

Indicates whether ignoring useless shapes.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### Remarks

Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

### Examples

```csharp
// Called: options.IgnoreUselessShapes = true;
public void LoadOptions_Property_IgnoreUselessShapes()
{
    LoadOptions options = new LoadOptions();
    options.IgnoreUselessShapes = true;
    var workbook = new Workbook(Path.Combine(Constants.sourcePath, "example.xlsx"), options);
    Assert.AreEqual(2, workbook.Worksheets[0].Shapes.Count);
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


