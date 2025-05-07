---
title: FormatCondition.DataBar
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Get the conditional formattings DataBar instance. The default instances color is blue. Valid only for type is DataBar
type: docs
url: /net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar.

```csharp
public DataBar DataBar { get; }
```

### Examples

```csharp
// Called: DataBarBorderType barborder = fc.DataBar.BarBorder.Type;
[Test]
        public void Property_DataBar()
        {
            String filePath = Constants.sourcePath + "ConditionalFormattings\\TestConditionalDefault.xlsx";
            Workbook _book = new Workbook(filePath);


            //FormatConditionCollection conds = GetFormatCondition("E3:G4", Color.LightGreen, _sheet);
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
            if (fcs.Count > 0)
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

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


