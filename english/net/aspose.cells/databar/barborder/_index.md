---
title: DataBar.BarBorder
second_title: Aspose.Cells for .NET API Reference
description: DataBar property. Gets an object that specifies the border of a data bar
type: docs
url: /net/aspose.cells/databar/barborder/
---
## DataBar.BarBorder property

Gets an object that specifies the border of a data bar.

```csharp
public DataBarBorder BarBorder { get; }
```

### Examples

```csharp
// Called: Color borderColor = fc.DataBar.BarBorder.Color;
[Test]
        public void Property_BarBorder()
        {
            String filePath = Constants.sourcePath + &quot;ConditionalFormattings\\TestConditionalDefault.xlsx&quot;;
            Workbook _book = new Workbook(filePath);


            //FormatConditionCollection conds = GetFormatCondition(&quot;E3:G4&quot;, Color.LightGreen, _sheet);
            //int idx = conds.AddCondition(FormatConditionType.DataBar);
            //FormatCondition cond = conds[idx];
            //cond.DataBar.Color = Color.Orange;
            //cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            //cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            //cond.DataBar.ShowValue = false;

            //cond.DataBar.BarBorder.Type = DataBarBorderType.DataBarBorderSolid;
            //cond.DataBar.BarBorder.Color = Color.Plum;

            //cond.DataBar.BarFillType = DataBarFillType.DataBarFillGradient;

            //cond.DataBar.AxisColor = Color.Red;
            //cond.DataBar.AxisPosition = DataBarAxisPosition.DataBarAxisAutomatic;

            //cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.DataBarColor;
            //cond.DataBar.NegativeBarFormat.Color = Color.White;

            //cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.DataBarColor;
            //cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            // _book.Save(filePath, SaveFormat.Xlsx);
            //read
            
            Worksheet _sheet = _book.Worksheets[0];
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

           AssertHelper.AreEqual(databarColor, Color.FromArgb(99, 142, 198));//Color.Orange);

            Assert.AreEqual(showValue, true);
            Assert.AreEqual(barborder, DataBarBorderType.None);

           AssertHelper.AreEqual(borderColor, Color.Empty);//Color.FromArgb(0, 221, 160, 221));

            Assert.AreEqual(barFilltype, DataBarFillType.Solid);

           AssertHelper.AreEqual(axisColor, Color.FromArgb( 0, 0, 0));

            Assert.AreEqual(axisPosition, DataBarAxisPosition.Automatic);
            Assert.AreEqual(negColorType, DataBarNegativeColorType.Color);

           AssertHelper.AreEqual(negColor, Color.FromArgb( 255, 0, 0));

            Assert.AreEqual(negBorderColorType, DataBarNegativeColorType.SameAsPositive);

           AssertHelper.AreEqual(negBorderColor, Color.FromArgb( 0, 0, 0));
        }
```

### See Also

* class [DataBarBorder](../../databarborder/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


