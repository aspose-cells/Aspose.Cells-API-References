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
public void Property_IgnoreUselessShapes(string file)
            {
                DefaultWarningCallback warningCallback = new DefaultWarningCallback();
                LoadOptions options = new LoadOptions();
                options.IgnoreUselessShapes = true;
                options.WarningCallback = warningCallback;
                Workbook wb = new Workbook(file, options);
                Util.SaveAsBuffer(wb, Util.GetSaveFormat(wb.FileFormat));
            }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


