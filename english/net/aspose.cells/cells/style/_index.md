---
title: Cells.Style
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets and sets the default style of the worksheet
type: docs
url: /net/aspose.cells/cells/style/
---
## Cells.Style property

Gets and sets the default style of the worksheet.

```csharp
public Style Style { get; set; }
```

### Examples

```csharp
// Called: Style style = cells.Style;
public void Cells_Property_Style()
{
    Workbook wb = new Workbook();
    wb.Settings.Region = CountryCode.Japan;
    Cells cells = wb.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    cell.Formula = "TEXT(43368, \"yyyymmdd!y\")";
    wb.CalculateFormula(false);
    Assert.AreEqual("20180925y", cell.Value, "Calculated result of TEXT(43368, \"yyyymmdd!y\")");

    cell.PutValue(43368);
    Style style = cells.Style;
    style.CultureCustom = "yyyymmdd!y";
    cell.SetStyle(style);
    Assert.AreEqual("20180925y", cell.StringValue, "Style.CultureCustom as \"yyyymmdd!y\"");
}
```

### See Also

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


