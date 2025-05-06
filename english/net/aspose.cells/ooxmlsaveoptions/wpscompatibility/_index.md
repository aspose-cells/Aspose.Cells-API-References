---
title: OoxmlSaveOptions.WpsCompatibility
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. Indicates whether to make the xls more compatible with WPS
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/wpscompatibility/
---
## OoxmlSaveOptions.WpsCompatibility property

Indicates whether to make the xls more compatible with WPS.

```csharp
public bool WpsCompatibility { get; set; }
```

### Examples

```csharp
// Called: saveOptions.WpsCompatibility = true;
[Test]
        public void Property_WpsCompatibility()
        {
            Workbook wkb = new Workbook();
            Cells cells = wkb.Worksheets[0].Cells;
            cells[&quot;A1&quot;].EmbeddedImage = File.ReadAllBytes(Constants.sourcePath + &quot;image1.jpg&quot;); //cells[&quot;A2&quot;].Formula = &quot;=C1&quot;;
            Style style = wkb.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            cells[&quot;A1&quot;].SetStyle(style);
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.WpsCompatibility = true;
            wkb.Settings.FormulaSettings.CalculateOnOpen = false;
            wkb.Save(Constants.destPath + &quot;CELLSNET57653.xlsx&quot;, saveOptions);
            wkb = new Workbook(Constants.destPath + &quot;CELLSNET57653.xlsx&quot;);
            Cell cell = wkb.Worksheets[0].Cells[&quot;A1&quot;];
            Assert.IsTrue(cell.EmbeddedImage != null);
           // Assert.IsTrue(cell.IsFormula);
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


