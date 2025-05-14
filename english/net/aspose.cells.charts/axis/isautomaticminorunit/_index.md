---
title: Axis.IsAutomaticMinorUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Indicates whether the minor unit of the axis is automatically assigned
type: docs
url: /net/aspose.cells.charts/axis/isautomaticminorunit/
---
## Axis.IsAutomaticMinorUnit property

Indicates whether the minor unit of the axis is automatically assigned.

```csharp
public bool IsAutomaticMinorUnit { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cAxisSrc.IsAutomaticMinorUnit, cAxisDest.IsAutomaticMinorUnit, info + ".IsAutomaticMinorUnit");
public static void Axis_Property_IsAutomaticMinorUnit(Axis cAxisSrc, Axis cAxisDest, string info)
        {
            if (AssertHelper.checkNull(cAxisSrc, cAxisDest, info))
            {
                return;
            }
            TitleTest.Axis_Property_IsAutomaticMinorUnit(cAxisSrc.Title, cAxisDest.Title, info + ".Title");
            AssertHelper.AreEqual(cAxisSrc.IsVisible, cAxisDest.IsVisible, info + ".IsVisible");
            if (cAxisSrc.IsVisible && cAxisDest.IsVisible)
            {
                //=================Axis Options================//
                //for valueaxis
                AssertHelper.AreEqual(cAxisSrc.IsAutomaticMinValue, cAxisDest.IsAutomaticMinValue, info + ".IsAutomaticMinValue");
                AssertHelper.AreEqual(cAxisSrc.MinValue, cAxisDest.MinValue, info + ".MinValue");
                AssertHelper.AreEqual(cAxisSrc.IsAutomaticMaxValue, cAxisDest.IsAutomaticMaxValue, info + ".IsAutomaticMaxValue");
                AssertHelper.AreEqual(cAxisSrc.MaxValue, cAxisDest.MaxValue, info + ".MaxValue");
                AssertHelper.AreEqual(cAxisSrc.IsAutomaticMajorUnit, cAxisDest.IsAutomaticMajorUnit, info + ".IsAutomaticMajorUnit");
                AssertHelper.AreEqual(cAxisSrc.MajorUnit, cAxisDest.MajorUnit, info + ".MajorUnit");
                AssertHelper.AreEqual(cAxisSrc.IsAutomaticMinorUnit, cAxisDest.IsAutomaticMinorUnit, info + ".IsAutomaticMinorUnit");
                AssertHelper.AreEqual(cAxisSrc.MinorUnit, cAxisDest.MinorUnit, info + ".MinorUnit");
                AssertHelper.AreEqual(cAxisSrc.IsPlotOrderReversed, cAxisDest.IsPlotOrderReversed, info + ".IsPlotOrderReversed");
                AssertHelper.AreEqual(cAxisSrc.IsLogarithmic, cAxisDest.IsLogarithmic, info + ".IsLogarithmic");
                AssertHelper.AreEqual(cAxisSrc.LogBase, cAxisDest.LogBase, info + ".LogBase");
                AssertHelper.AreEqual(cAxisSrc.DisplayUnit, cAxisDest.DisplayUnit, info + ".DisplayUnit");
                if (cAxisSrc.DisplayUnit != DisplayUnitType.None)
                {
                    DisplayUnitLabelTest.Axis_Property_IsAutomaticMinorUnit(cAxisSrc.DisplayUnitLabel, cAxisDest.DisplayUnitLabel, info + ".DisplayUnitLabel");
                }
                AssertHelper.AreEqual(cAxisSrc.MajorTickMark, cAxisDest.MajorTickMark, info + ".MajorTickMark");
                AssertHelper.AreEqual(cAxisSrc.MinorTickMark, cAxisDest.MinorTickMark, info + ".MinorTickMark");
                AssertHelper.AreEqual(cAxisSrc.TickLabelPosition, cAxisDest.TickLabelPosition, info + ".TickLabelPosition");
                AssertHelper.AreEqual(cAxisSrc.CrossType, cAxisDest.CrossType, info + ".CrossType");
                switch (cAxisSrc.CrossType)
                {
                    case CrossType.Automatic:
                        break;
                    case CrossType.Custom:
                        AssertHelper.AreEqual(cAxisSrc.CrossAt, cAxisDest.CrossAt, info + ".CrossAt");
                        break;
                    case CrossType.Maximum:                        
                        break;
                }

                /*-----additional(Y Axis)---*/
                AssertHelper.AreEqual(cAxisSrc.TickMarkSpacing, cAxisDest.TickMarkSpacing, info + ".TickMarkSpacing");
                AssertHelper.AreEqual(cAxisSrc.TickLabelSpacing, cAxisDest.TickLabelSpacing, info + ".TickLabelSpacing");
                AssertHelper.AreEqual(cAxisSrc.AxisBetweenCategories, cAxisDest.AxisBetweenCategories, info + ".AxisBetweenCategories");
                AssertHelper.AreEqual(cAxisSrc.CategoryType, cAxisDest.CategoryType, info + ".CategoryType");
                if (cAxisSrc.CategoryType == CategoryType.TimeScale)
                {
                    AssertHelper.AreEqual(cAxisSrc.BaseUnitScale, cAxisDest.BaseUnitScale, info + ".BaseUnitScale");
                }
                //=====================Number Option==================//
                AssertHelper.AreEqual(cAxisSrc.TickLabels.NumberFormatLinked, cAxisDest.TickLabels.NumberFormatLinked, info + ".TickLabels.NumberFormatLinked");
                if (cAxisSrc.TickLabels.NumberFormatLinked == false)
                {
                    AssertHelper.AreEqual(cAxisSrc.TickLabels.Number, cAxisDest.TickLabels.Number, info + ".TickLabels.Number");
                    AssertHelper.AreEqual(cAxisSrc.TickLabels.NumberFormat, cAxisDest.TickLabels.NumberFormat, info + ".TickLabels.NumberFormat");
                }                
                AssertHelper.AreEqual(cAxisSrc.TickLabels.Offset, cAxisDest.TickLabels.Offset, info + ".TickLabels.Offset");
                //=====================Fill Option======================//
               
                //=====================Alignment Option=================//
                AssertHelper.AreEqual(cAxisSrc.TickLabels.ReadingOrder, cAxisDest.TickLabels.ReadingOrder, info + ".TickLabels.TextDirection");
                AssertHelper.AreEqual(cAxisSrc.TickLabels.RotationAngle, cAxisDest.TickLabels.RotationAngle, info + ".TickLabels.RotationAngle");
                

                //==============compare patterns==============//
                LineTest.Axis_Property_IsAutomaticMinorUnit(cAxisSrc.AxisLine, cAxisDest.AxisLine, info + ".AxisLine");

                //==============compare font================//
                FontTest.Axis_Property_IsAutomaticMinorUnit(cAxisSrc.TickLabels.Font, cAxisDest.TickLabels.Font, info + ".TickLabels.Font");
                AssertHelper.AreEqual(cAxisSrc.TickLabels.AutoScaleFont, cAxisDest.TickLabels.AutoScaleFont, info + ".TickLabels.AutoScaleFont");
                AssertHelper.AreEqual(cAxisSrc.TickLabels.BackgroundMode, cAxisDest.TickLabels.BackgroundMode, info + ".TickLabels.Background");
              
                
                //==============compare scale=================//
                //AssertHelper.AreEqual(cAxisSrc.CrossAt, cAxisDest.CrossAt, info + ".CrossAt");
                //AssertHelper.AreEqual(cAxisSrc.TickLabelSpacing, cAxisDest.TickLabelSpacing, info + ".TickLabelSpacing");
                //AssertHelper.AreEqual(cAxisSrc.TickMarkSpacing, cAxisDest.TickMarkSpacing, info + ".TickMarkSpacing");
                //AssertHelper.AreEqual(cAxisSrc.AxisBetweenCategories, cAxisDest.AxisBetweenCategories, info + ".AxisBetweenCategories");
                //AssertHelper.AreEqual(cAxisSrc.IsPlotOrderReversed, cAxisDest.IsPlotOrderReversed, info + ".IsPlotOrderReversed");
                //AssertHelper.AreEqual(cAxisSrc.DisplayUnit, cAxisDest.DisplayUnit, info + ".DisplayUnit");
                //AssertHelper.AreEqual(cAxisSrc.IsLogarithmic, cAxisDest.IsLogarithmic, info + ".IsLogarithmic");
                ////AssertHelper.AreEqual(vAxisSrc.IsPlotOrderReversed, vAxisDest.IsPlotOrderReversed, info + ".IsPlotOrderReversed");
                //AssertHelper.AreEqual(cAxisSrc.CrossType, cAxisDest.CrossType, info + ".CrossType");
                //===//
                //AssertHelper.AreEqual(cAxisSrc.MinValue, cAxisDest.MinValue, info + ".MinValue");
                //AssertHelper.AreEqual(cAxisSrc.MaxValue, cAxisDest.MaxValue, info + ".MaxValue");
                //AssertHelper.AreEqual(cAxisSrc.BaseUnitScale, cAxisDest.BaseUnitScale, info + ".BaseUnitScale");
                //AssertHelper.AreEqual(cAxisSrc.MajorUnit, cAxisDest.MajorUnit, info + ".MajorUnit");
                //AssertHelper.AreEqual(cAxisSrc.MajorUnitScale, cAxisDest.MajorUnitScale, info + ".MajorUnitScale");
                //AssertHelper.AreEqual(cAxisSrc.MinorUnit, cAxisDest.MinorUnit, info + ".MinorUnit");
                //AssertHelper.AreEqual(cAxisSrc.MinorUnitScale, cAxisDest.MinorUnitScale, info + ".MinorUnitScale");              
               
                ////==============compare number===============//
                //AssertHelper.AreEqual(cAxisSrc.TickLabels.NumberFormatLinked, cAxisDest.TickLabels.NumberFormatLinked, info + ".TickLabels.NumberFormatLinked");
                //if (cAxisSrc.TickLabels.NumberFormatLinked == false && cAxisDest.TickLabels.NumberFormatLinked == false)
                //{
                //    AssertHelper.AreEqual(cAxisSrc.TickLabels.Number, cAxisDest.TickLabels.Number, info + ".TickLabels.Number");
                //    AssertHelper.AreEqual(cAxisSrc.TickLabels.NumberFormat, cAxisDest.TickLabels.NumberFormat, info + ".TickLabels.NumberFormat");
                //}
                ////==============compare alignment=============//
                //AssertHelper.AreEqual(cAxisSrc.TickLabels.TextDirection, cAxisDest.TickLabels.TextDirection, info + ".TickLabels.TextDirection");
                //AssertHelper.AreEqual(cAxisSrc.TickLabels.RotationAngle, cAxisDest.TickLabels.RotationAngle, info + ".TickLabels.RotationAngle");
                //AssertHelper.AreEqual(cAxisSrc.TickLabels.Offset, cAxisDest.TickLabels.Offset, info + ".TickLabels.Offset");
            } 
            LineTest.Axis_Property_IsAutomaticMinorUnit(cAxisSrc.MajorGridLines, cAxisDest.MajorGridLines, info+".MajorGridLines");
            LineTest.Axis_Property_IsAutomaticMinorUnit(cAxisSrc.MinorGridLines, cAxisDest.MinorGridLines, info+".MinorGridLines");
            //AssertHelper.AreEqual(cAxisSrc.CategoryType, cAxisDest.CategoryType, info + ".CategoryType");
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


