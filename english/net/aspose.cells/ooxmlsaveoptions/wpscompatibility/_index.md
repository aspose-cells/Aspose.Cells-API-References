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

            Workbook wkb = new Workbook(Constants.sourcePath + "CELLSNET57653_1.xlsx");
            Cells cells = wkb.Worksheets[0].Cells;
            cells["A1"].EmbeddedImage = File.ReadAllBytes(Constants.sourcePath + "image1.jpg"); //cells["A2"].Formula = "=C1";
            Style style = wkb.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            cells["A1"].SetStyle(style);
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.WpsCompatibility = true;
            wkb.Settings.FormulaSettings.CalculateOnOpen = false;
            wkb.Save(Constants.destPath + "CELLSNET57653.xlsx", saveOptions);
            wkb = new Workbook(Constants.destPath + "CELLSNET57653.xlsx");
            Cell cell = wkb.Worksheets[0].Cells["A1"];
            Assert.IsTrue(cell.EmbeddedImage != null);
           // Assert.IsTrue(cell.IsFormula);
            Assert.AreEqual("=B2", wkb.Worksheets[0].Cells["D2"].Formula);

        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


