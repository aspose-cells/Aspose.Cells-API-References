---
title: FormulaSettings.PreservePaddingSpaces
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false
type: docs
url: /net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Remarks

Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.

### Examples

```csharp
// Called: excel.Settings.FormulaSettings.PreservePaddingSpaces ? fml : fml.Replace(" ", ""));
public void FormulaSettings_Property_PreservePaddingSpaces()
{
    Workbook excel = new Workbook(Constants.sourcePath + "example.xlsx");
    excel.Worksheets[1].Cells.DeleteColumn(0, true) ;
    excel.Worksheets[1].Cells.DeleteRows(0, 1, true);
    string fml = "=SUM(IF(Data!B2:B6=\"A\", Data!C2:C5, 0))";
    Assert.AreEqual(excel.Worksheets[0].Cells["C3"].Formula,
        excel.Settings.FormulaSettings.PreservePaddingSpaces ? fml : fml.Replace(" ", ""));
    Assert.AreEqual(excel.Worksheets[1].AutoFilter.Range, "B1:C1");
    excel.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


