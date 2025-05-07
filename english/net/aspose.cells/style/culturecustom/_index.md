---
title: Style.CultureCustom
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets and sets the culturedependent pattern string for number format. If no number format has been set for this object null will be returned. If number format is builtin the pattern string corresponding to the builtin number will be returned
type: docs
url: /net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```csharp
public string CultureCustom { get; set; }
```

### Remarks

For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified.

### Examples

```csharp
// Called: lc_Style.CultureCustom = "@"; //'書式を文字列に変更
[Test]
        public void Property_CultureCustom()
        {
            Workbook lc_Workbook = new Workbook(Constants.sourcePath +"CELLSNET50377.xls");
            Aspose.Cells.Range lc_Range = lc_Workbook.Worksheets[0].Cells.CreateRange(1, 1, 1, 1);
            Style lc_Style = lc_Range[0, 0].GetStyle();
            Color c = lc_Style.ForegroundColor;
            lc_Style.CultureCustom = "@"; //'書式を文字列に変更

            StyleFlag lc_Flag = new StyleFlag();
            lc_Flag.NumberFormat = true;

             lc_Range.ApplyStyle(lc_Style, lc_Flag);
            lc_Style = lc_Range[0, 0].GetStyle();
            lc_Workbook.Save(Constants.destPath + "CELLSNET50377.xlsx");
            Workbook workbook = new Workbook(Constants.destPath + "CELLSNET50377.xlsx");
            Cell cell = workbook.Worksheets[0].Cells["B2"];
            lc_Style = cell.GetStyle();
            Assert.AreEqual("@", lc_Style.Custom);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


