---
title: NegativeBarFormat.BorderColorType
second_title: Aspose.Cells for .NET API Reference
description: NegativeBarFormat property. Gets whether to use the same border color as positive data bars
type: docs
url: /net/aspose.cells/negativebarformat/bordercolortype/
---
## NegativeBarFormat.BorderColorType property

Gets whether to use the same border color as positive data bars.

```csharp
public DataBarNegativeColorType BorderColorType { get; set; }
```

### Examples

```csharp
// Called: cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
[Test]
        public void Property_BorderColorType()
        {
            //String filePath = Constants.destPath + &quot;Test4Conditionaldest.xlsx&quot;;
            Workbook _book = new Workbook();
            Worksheet _sheet = _book.Worksheets[0];

            FormatConditionCollection conds = GetFormatCondition(&quot;E3:G4&quot;, Color.LightGreen, _sheet);
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            cond.DataBar.BarFillType = DataBarFillType.Solid;

            cond.DataBar.AxisColor = Color.Red;
            cond.DataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;

            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            //_book.Save(filePath, SaveFormat.Xlsx);
            //read
            _book = Util.ReSave(_book, SaveFormat.Xlsx);// new Workbook(filePath);
            _sheet = _book.Worksheets[0];

            FormatConditionCollection fcs = _sheet.ConditionalFormattings[0];
            FormatCondition fc = null;
            if (fcs.Count &gt; 0)
                fc = fcs[0];

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

            Assert.AreEqual(minType, FormatConditionValueType.AutomaticMin);
            Assert.AreEqual(maxType, FormatConditionValueType.AutomaticMax);

            Assert.AreEqual(databarColor, Color.FromArgb(255, 165, 0));//Color.Orange);

            Assert.AreEqual(showValue, false);
            Assert.AreEqual(barborder, DataBarBorderType.Solid);

           AssertHelper.AreEqual(borderColor, Color.FromArgb(221, 160, 221));

            Assert.AreEqual(barFilltype, DataBarFillType.Solid);

           AssertHelper.AreEqual(axisColor, Color.FromArgb(255, 0, 0));

            Assert.AreEqual(axisPosition, DataBarAxisPosition.Midpoint);
            Assert.AreEqual(negColorType, DataBarNegativeColorType.Color);

           AssertHelper.AreEqual(negColor, Color.FromArgb(255, 255, 255));

            Assert.AreEqual(negBorderColorType, DataBarNegativeColorType.Color);

           AssertHelper.AreEqual(negBorderColor, Color.FromArgb(255, 255, 0));
        }
```

### See Also

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


