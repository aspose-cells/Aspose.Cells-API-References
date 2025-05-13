---
title: Style.SetTwoColorGradient
second_title: Aspose.Cells for .NET API Reference
description: Style method. Sets the specified fill to a twocolor gradient
type: docs
url: /net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

Sets the specified fill to a two-color gradient.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| gradientStyleType | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### Examples

```csharp
// Called: fc.Style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);
public void Style_Method_SetTwoColorGradient()
{
    Workbook wb = new Workbook();
    ConditionalFormattingCollection cfc = wb.Worksheets[0].ConditionalFormattings;
    FormatConditionCollection fcc = cfc[cfc.Add()];
    fcc.AddArea(CellArea.CreateCellArea(0, 0, 0, 0));
    FormatCondition fc = fcc[fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "1", null)];
    fc.Style.Font.Size = 26;
    fc.Style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);
    Cell cell = wb.Worksheets[0].Cells[0, 0];
    cell.PutValue(2);
    Style ds = cell.GetDisplayStyle();
    Assert.AreEqual(26, ds.Font.Size, "A1.DisplayStyle.Font with one condition");
    Color c1, c2;
    GradientStyleType gst;
    int sv;
    ds.GetTwoColorGradient(out c1, out c2, out gst, out sv);
    AssertHelper.AreEqual(Color.Green, c1, "A1.DisplayStyle.Color1 with one condition");
    AssertHelper.AreEqual(Color.Red, c2, "A1.DisplayStyle.Color2 with one condition");
    AssertHelper.AreEqual(GradientStyleType.Vertical, gst, "A1.DisplayStyle.GradientStyleType with one condition");
    AssertHelper.AreEqual(1, sv, "A1.DisplayStyle.Variant with one condition");
    fc = fcc[fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "0", null)];
    fc.Style.SetTwoColorGradient(Color.Blue, Color.Gray, GradientStyleType.Horizontal, 2);
    ds = cell.GetDisplayStyle();
    Assert.AreEqual(26, ds.Font.Size, "A1.DisplayStyle.Font with two conditions");
    ds.GetTwoColorGradient(out c1, out c2, out gst, out sv);
    AssertHelper.AreEqual(Color.Blue, c1, "A1.DisplayStyle.Color1 with two conditions");
    AssertHelper.AreEqual(Color.Gray, c2, "A1.DisplayStyle.Color2 with two conditions");
    AssertHelper.AreEqual(GradientStyleType.Horizontal, gst, "A1.DisplayStyle.GradientStyleType with two conditions");
    AssertHelper.AreEqual(2, sv, "A1.DisplayStyle.Variant with two conditions");
}
```

### See Also

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


