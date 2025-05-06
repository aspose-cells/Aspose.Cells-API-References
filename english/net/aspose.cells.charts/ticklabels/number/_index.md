---
title: TickLabels.Number
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Represents the format number for the TickLabels object
type: docs
url: /net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

Represents the format number for the TickLabels object.

```csharp
public int Number { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cAxisSrc.TickLabels.Number, cAxisDest.TickLabels.Number, info + &amp;quot;.TickLabels.Number&amp;quot;);
public static void Property_Number(Axis cAxisSrc, Axis cAxisDest, string info)
        {
            if (AssertHelper.checkNull(cAxisSrc, cAxisDest, info))
            {
                return;
            }
            TitleTest.Property_Number(cAxisSrc.Title, cAxisDest.Title, info + &quot;.Title&quot;);
            AssertHelper.AreEqual(cAxisSrc.IsVisible, cAxisDest.IsVisible, info + &quot;.IsVisible&quot;);
            if (cAxisSrc.IsVisible &amp;&amp; cAxisDest.IsVisible)
            {
                //=================Axis Options================//
                //for valueaxis
                AssertHelper.AreEqual(cAxisSrc.IsAutomaticMinValue, cAxisDest.IsAutomaticMinValue, info + &quot;.IsAutomaticMinValue&quot;);
                AssertHelper.AreEqual(cAxisSrc.MinValue, cAxisDest.MinValue, info + &quot;.MinValue&quot;);
                AssertHelper.AreEqual(cAxisSrc.IsAutomaticMaxValue, cAxisDest.IsAutomaticMaxValue, info + &quot;.IsAutomaticMaxValue&quot;);
                AssertHelper.AreEqual(cAxisSrc.MaxValue, cAxisDest.MaxValue, info + &quot;.MaxValue&quot;);
                AssertHelper.AreEqual(cAxisSrc.IsAutomaticMajorUnit, cAxisDest.IsAutomaticMajorUnit, info + &quot;.IsAutomaticMajorUnit&quot;);
                AssertHelper.AreEqual(cAxisSrc.MajorUnit, cAxisDest.MajorUnit, info + &quot;.MajorUnit&quot;);
                AssertHelper.AreEqual(cAxisSrc.IsAutomaticMinorUnit, cAxisDest.IsAutomaticMinorUnit, info + &quot;.IsAutomaticMinorUnit&quot;);
                AssertHelper.AreEqual(cAxisSrc.MinorUnit, cAxisDest.MinorUnit, info + &quot;.MinorUnit&quot;);
                AssertHelper.AreEqual(cAxisSrc.IsPlotOrderReversed, cAxisDest.IsPlotOrderReversed, info + &quot;.IsPlotOrderReversed&quot;);
                AssertHelper.AreEqual(cAxisSrc.IsLogarithmic, cAxisDest.IsLogarithmic, info + &quot;.IsLogarithmic&quot;);
                AssertHelper.AreEqual(cAxisSrc.LogBase, cAxisDest.LogBase, info + &quot;.LogBase&quot;);
                AssertHelper.AreEqual(cAxisSrc.DisplayUnit, cAxisDest.DisplayUnit, info + &quot;.DisplayUnit&quot;);
                if (cAxisSrc.DisplayUnit != DisplayUnitType.None)
                {
                    DisplayUnitLabelTest.Property_Number(cAxisSrc.DisplayUnitLabel, cAxisDest.DisplayUnitLabel, info + &quot;.DisplayUnitLabel&quot;);
                }
                AssertHelper.AreEqual(cAxisSrc.MajorTickMark, cAxisDest.MajorTickMark, info + &quot;.MajorTickMark&quot;);
                AssertHelper.AreEqual(cAxisSrc.MinorTickMark, cAxisDest.MinorTickMark, info + &quot;.MinorTickMark&quot;);
                AssertHelper.AreEqual(cAxisSrc.TickLabelPosition, cAxisDest.TickLabelPosition, info + &quot;.TickLabelPosition&quot;);
                AssertHelper.AreEqual(cAxisSrc.CrossType, cAxisDest.CrossType, info + &quot;.CrossType&quot;);
                switch (cAxisSrc.CrossType)
                {
                    case CrossType.Automatic:
                        break;
                    case CrossType.Custom:
                        AssertHelper.AreEqual(cAxisSrc.CrossAt, cAxisDest.CrossAt, info + &quot;.CrossAt&quot;);
                        break;
                    case CrossType.Maximum:                        
                        break;
                }

                /*-----additional(Y Axis)---*/
                AssertHelper.AreEqual(cAxisSrc.TickMarkSpacing, cAxisDest.TickMarkSpacing, info + &quot;.TickMarkSpacing&quot;);
                AssertHelper.AreEqual(cAxisSrc.TickLabelSpacing, cAxisDest.TickLabelSpacing, info + &quot;.TickLabelSpacing&quot;);
                AssertHelper.AreEqual(cAxisSrc.AxisBetweenCategories, cAxisDest.AxisBetweenCategories, info + &quot;.AxisBetweenCategories&quot;);
                AssertHelper.AreEqual(cAxisSrc.CategoryType, cAxisDest.CategoryType, info + &quot;.CategoryType&quot;);
                if (cAxisSrc.CategoryType == CategoryType.TimeScale)
                {
                    AssertHelper.AreEqual(cAxisSrc.BaseUnitScale, cAxisDest.BaseUnitScale, info + &quot;.BaseUnitScale&quot;);
                }
                //=====================Number Option==================//
                AssertHelper.AreEqual(cAxisSrc.TickLabels.NumberFormatLinked, cAxisDest.TickLabels.NumberFormatLinked, info + &quot;.TickLabels.NumberFormatLinked&quot;);
                if (cAxisSrc.TickLabels.NumberFormatLinked == false)
                {
                    AssertHelper.AreEqual(cAxisSrc.TickLabels.Number, cAxisDest.TickLabels.Number, info + &quot;.TickLabels.Number&quot;);
                    AssertHelper.AreEqual(cAxisSrc.TickLabels.NumberFormat, cAxisDest.TickLabels.NumberFormat, info + &quot;.TickLabels.NumberFormat&quot;);
                }                
                AssertHelper.AreEqual(cAxisSrc.TickLabels.Offset, cAxisDest.TickLabels.Offset, info + &quot;.TickLabels.Offset&quot;);
                //=====================Fill Option======================//
               
                //=====================Alignment Option=================//
                AssertHelper.AreEqual(cAxisSrc.TickLabels.ReadingOrder, cAxisDest.TickLabels.ReadingOrder, info + &quot;.TickLabels.TextDirection&quot;);
                AssertHelper.AreEqual(cAxisSrc.TickLabels.RotationAngle, cAxisDest.TickLabels.RotationAngle, info + &quot;.TickLabels.RotationAngle&quot;);
                

                //==============compare patterns==============//
                LineTest.Property_Number(cAxisSrc.AxisLine, cAxisDest.AxisLine, info + &quot;.AxisLine&quot;);

                //==============compare font================//
                FontTest.Property_Number(cAxisSrc.TickLabels.Font, cAxisDest.TickLabels.Font, info + &quot;.TickLabels.Font&quot;);
                AssertHelper.AreEqual(cAxisSrc.TickLabels.AutoScaleFont, cAxisDest.TickLabels.AutoScaleFont, info + &quot;.TickLabels.AutoScaleFont&quot;);
                AssertHelper.AreEqual(cAxisSrc.TickLabels.BackgroundMode, cAxisDest.TickLabels.BackgroundMode, info + &quot;.TickLabels.Background&quot;);
              
                
                //==============compare scale=================//
                //AssertHelper.AreEqual(cAxisSrc.CrossAt, cAxisDest.CrossAt, info + &quot;.CrossAt&quot;);
                //AssertHelper.AreEqual(cAxisSrc.TickLabelSpacing, cAxisDest.TickLabelSpacing, info + &quot;.TickLabelSpacing&quot;);
                //AssertHelper.AreEqual(cAxisSrc.TickMarkSpacing, cAxisDest.TickMarkSpacing, info + &quot;.TickMarkSpacing&quot;);
                //AssertHelper.AreEqual(cAxisSrc.AxisBetweenCategories, cAxisDest.AxisBetweenCategories, info + &quot;.AxisBetweenCategories&quot;);
                //AssertHelper.AreEqual(cAxisSrc.IsPlotOrderReversed, cAxisDest.IsPlotOrderReversed, info + &quot;.IsPlotOrderReversed&quot;);
                //AssertHelper.AreEqual(cAxisSrc.DisplayUnit, cAxisDest.DisplayUnit, info + &quot;.DisplayUnit&quot;);
                //AssertHelper.AreEqual(cAxisSrc.IsLogarithmic, cAxisDest.IsLogarithmic, info + &quot;.IsLogarithmic&quot;);
                ////AssertHelper.AreEqual(vAxisSrc.IsPlotOrderReversed, vAxisDest.IsPlotOrderReversed, info + &quot;.IsPlotOrderReversed&quot;);
                //AssertHelper.AreEqual(cAxisSrc.CrossType, cAxisDest.CrossType, info + &quot;.CrossType&quot;);
                //===//
                //AssertHelper.AreEqual(cAxisSrc.MinValue, cAxisDest.MinValue, info + &quot;.MinValue&quot;);
                //AssertHelper.AreEqual(cAxisSrc.MaxValue, cAxisDest.MaxValue, info + &quot;.MaxValue&quot;);
                //AssertHelper.AreEqual(cAxisSrc.BaseUnitScale, cAxisDest.BaseUnitScale, info + &quot;.BaseUnitScale&quot;);
                //AssertHelper.AreEqual(cAxisSrc.MajorUnit, cAxisDest.MajorUnit, info + &quot;.MajorUnit&quot;);
                //AssertHelper.AreEqual(cAxisSrc.MajorUnitScale, cAxisDest.MajorUnitScale, info + &quot;.MajorUnitScale&quot;);
                //AssertHelper.AreEqual(cAxisSrc.MinorUnit, cAxisDest.MinorUnit, info + &quot;.MinorUnit&quot;);
                //AssertHelper.AreEqual(cAxisSrc.MinorUnitScale, cAxisDest.MinorUnitScale, info + &quot;.MinorUnitScale&quot;);              
               
                ////==============compare number===============//
                //AssertHelper.AreEqual(cAxisSrc.TickLabels.NumberFormatLinked, cAxisDest.TickLabels.NumberFormatLinked, info + &quot;.TickLabels.NumberFormatLinked&quot;);
                //if (cAxisSrc.TickLabels.NumberFormatLinked == false &amp;&amp; cAxisDest.TickLabels.NumberFormatLinked == false)
                //{
                //    AssertHelper.AreEqual(cAxisSrc.TickLabels.Number, cAxisDest.TickLabels.Number, info + &quot;.TickLabels.Number&quot;);
                //    AssertHelper.AreEqual(cAxisSrc.TickLabels.NumberFormat, cAxisDest.TickLabels.NumberFormat, info + &quot;.TickLabels.NumberFormat&quot;);
                //}
                ////==============compare alignment=============//
                //AssertHelper.AreEqual(cAxisSrc.TickLabels.TextDirection, cAxisDest.TickLabels.TextDirection, info + &quot;.TickLabels.TextDirection&quot;);
                //AssertHelper.AreEqual(cAxisSrc.TickLabels.RotationAngle, cAxisDest.TickLabels.RotationAngle, info + &quot;.TickLabels.RotationAngle&quot;);
                //AssertHelper.AreEqual(cAxisSrc.TickLabels.Offset, cAxisDest.TickLabels.Offset, info + &quot;.TickLabels.Offset&quot;);
            } 
            LineTest.Property_Number(cAxisSrc.MajorGridLines, cAxisDest.MajorGridLines, info+&quot;.MajorGridLines&quot;);
            LineTest.Property_Number(cAxisSrc.MinorGridLines, cAxisDest.MinorGridLines, info+&quot;.MinorGridLines&quot;);
            //AssertHelper.AreEqual(cAxisSrc.CategoryType, cAxisDest.CategoryType, info + &quot;.CategoryType&quot;);
        }
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


