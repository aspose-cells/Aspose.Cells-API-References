---
title: FormulaSettings.CalculateOnOpen
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether the application is required to perform a full calculation when the workbook is opened
type: docs
url: /net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Indicates whether the application is required to perform a full calculation when the workbook is opened.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Remarks

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### Examples

```csharp
// Called: wkb.Settings.FormulaSettings.CalculateOnOpen = false;
public void FormulaSettings_Property_CalculateOnOpen()
{

    Workbook wkb = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = wkb.Worksheets[0].Cells;
    cells["A1"].EmbeddedImage = File.ReadAllBytes(Constants.sourcePath + "image1.jpg"); //cells["A2"].Formula = "=C1";
    Style style = wkb.CreateStyle();
    style.HorizontalAlignment = TextAlignmentType.Center;
    style.VerticalAlignment = TextAlignmentType.Center;
    cells["A1"].SetStyle(style);
    OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
    saveOptions.WpsCompatibility = true;
    wkb.Settings.FormulaSettings.CalculateOnOpen = false;
    wkb.Save(Constants.destPath + "example.xlsx", saveOptions);
    wkb = new Workbook(Constants.destPath + "example.xlsx");
    Cell cell = wkb.Worksheets[0].Cells["A1"];
    Assert.IsTrue(cell.EmbeddedImage != null);
   // Assert.IsTrue(cell.IsFormula);
    Assert.AreEqual("=B2", wkb.Worksheets[0].Cells["D2"].Formula);

}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


