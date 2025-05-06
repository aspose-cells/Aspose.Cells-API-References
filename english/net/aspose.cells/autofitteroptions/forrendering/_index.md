---
title: AutoFitterOptions.ForRendering
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Indicates whether fit for rendering purpose
type: docs
url: /net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

Indicates whether fit for rendering purpose.

```csharp
public bool ForRendering { get; set; }
```

### Examples

```csharp
// Called: autoFitterOptions.ForRendering= true;
[Test]
        public void Property_ForRendering()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-53267.xlsx&quot;);
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.ForRendering= true;
            wb.Worksheets[0].AutoFitRows(autoFitterOptions);

            Assert.AreEqual(247, wb.Worksheets[0].Cells.GetRowHeightPixel(0));
        }
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


