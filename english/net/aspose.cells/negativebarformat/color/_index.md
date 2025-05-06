---
title: NegativeBarFormat.Color
second_title: Aspose.Cells for .NET API Reference
description: NegativeBarFormat property. Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars
type: docs
url: /net/aspose.cells/negativebarformat/color/
---
## NegativeBarFormat.Color property

Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: Color negColor = fc.DataBar.NegativeBarFormat.Color;
[Test]
        public void Property_Color()
        {
            String sfilePath = Constants.sourcePath + &quot;ConditionalFormattings\\TestDataBarCopy.xlsx&quot;;
            String dfilePath = Constants.destPath + &quot;TestDataBarCopy2.xlsx&quot;;

            Workbook book = new Workbook(sfilePath);
            ConditionalFormattingCollection cfs = book.Worksheets[0].ConditionalFormattings;
            book.Worksheets[1].ConditionalFormattings.Copy(cfs);
            book.Save(dfilePath);
            Workbook newbook = new Workbook(dfilePath);
            ConditionalFormattingCollection newcfs = newbook.Worksheets[1].ConditionalFormattings;
            FormatConditionCollection fcs = newcfs[0];
            FormatCondition fc = fcs[0];

            FormatConditionValueType minType = fc.DataBar.MinCfvo.Type;
            FormatConditionValueType maxType = fc.DataBar.MaxCfvo.Type;
            Color databarColor = fc.DataBar.Color;
            bool showValue = fc.DataBar.ShowValue;

            DataBarBorderType barborder = fc.DataBar.BarBorder.Type;
            Color borderColor = fc.DataBar.BarBorder.Color;

            DataBarFillType barFilltype = fc.DataBar.BarFillType;

            Color axisColor = fc.DataBar.AxisColor;
            DataBarAxisPosition axisPosition = fc.DataBar.AxisPosition;

            DataBarNegativeColorType negColorType = fc.DataBar.NegativeBarFormat.ColorType;
            Color negColor = fc.DataBar.NegativeBarFormat.Color;

            DataBarNegativeColorType negBorderColorType = fc.DataBar.NegativeBarFormat.BorderColorType;
            Color negBorderColor = fc.DataBar.NegativeBarFormat.BorderColor;

            string sqref = GetCellAreaName(fcs.GetCellArea(0));

            Assert.AreEqual(minType, FormatConditionValueType.AutomaticMin);
            Assert.AreEqual(maxType, FormatConditionValueType.AutomaticMax);

           AssertHelper.AreEqual(databarColor, Color.FromArgb(255, 0, 0));//Color.Orange);

            Assert.AreEqual(showValue, true);

            Assert.AreEqual(barborder, DataBarBorderType.Solid);

           AssertHelper.AreEqual(borderColor, Color.FromArgb(0, 0, 0));

            Assert.AreEqual(barFilltype, DataBarFillType.Gradient);

           AssertHelper.AreEqual(axisColor, Color.FromArgb(0, 0, 0));

            Assert.AreEqual(axisPosition, DataBarAxisPosition.Midpoint);
            Assert.AreEqual(negColorType, DataBarNegativeColorType.SameAsPositive);

           AssertHelper.AreEqual(negColor, Color.FromArgb(255, 0, 0));

            Assert.AreEqual(negBorderColorType, DataBarNegativeColorType.Color);

           AssertHelper.AreEqual(negBorderColor, Color.FromArgb(228, 108, 10));

            Assert.AreEqual(sqref, &quot;A1:C1&quot;);
        }
```

### See Also

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


