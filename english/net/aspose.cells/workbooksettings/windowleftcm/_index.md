---
title: WorkbookSettings.WindowLeftCM
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. The distance from the left edge of the client area to the left edge of the window. In unit of centimeter
type: docs
url: /net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

```csharp
public double WindowLeftCM { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(expected.WindowLeftCM, result.WindowLeftCM, delta, info + &amp;quot;.WindowLeftCM&amp;quot;);
private static void Property_WindowLeftCM(WorkbookSettings expected, WorkbookSettings result, string info)
        {
            AssertHelper.AreEqual(expected.Date1904, result.Date1904, info + &quot;.Settings.Date1904&quot;);

            AssertHelper.AreEqual(expected.DisplayDrawingObjects, result.DisplayDrawingObjects, info + &quot;.Settings.DisplayDrawingObjects&quot;);

            AssertHelper.AreEqual(expected.IsHScrollBarVisible, result.IsHScrollBarVisible, info + &quot;.Settings.IsHScrollBarVisible&quot;);
            AssertHelper.AreEqual(expected.IsProtected, result.IsProtected, info + &quot;.Settings.IsProtected&quot;);
            AssertHelper.AreEqual(expected.IsVScrollBarVisible, result.IsVScrollBarVisible, info + &quot;.Settings.IsVScrollBarVisible&quot;);
            AssertHelper.AreEqual(expected.LanguageCode, result.LanguageCode, info + &quot;.Settings.LanguageCode&quot;);
            AssertHelper.AreEqual(expected.Password, result.Password, info + &quot;.Settings.Password&quot;);
            AssertHelper.AreEqual(expected.Region, result.Region, info + &quot;.Settings.Region&quot;);
            AssertHelper.AreEqual(expected.Shared, result.Shared, info + &quot;.Settings.Shared&quot;);
            AssertHelper.AreEqual(expected.ShowTabs, result.ShowTabs, info + &quot;.Settings.ShowTabs&quot;);
            AssertHelper.AreEqual(expected.DisplayDrawingObjects, result.DisplayDrawingObjects, info + &quot;.Settings.DisplayDrawingObjects&quot;);
            AssertHelper.AreEqual(expected.SheetTabBarWidth, result.SheetTabBarWidth, info + &quot;.SheetTabBarWidth&quot;);
            AssertHelper.AreEqual(expected.WindowHeightCM, result.WindowHeightCM, delta, info + &quot;.WindowHeightCM&quot;);
            AssertHelper.AreEqual(expected.WindowHeightInch, result.WindowHeightInch, delta, info + &quot;.WindowHeightInch&quot;);
            AssertHelper.AreEqual(expected.WindowLeftCM, result.WindowLeftCM, delta, info + &quot;.WindowLeftCM&quot;);
            AssertHelper.AreEqual(expected.WindowLeftInch, result.WindowLeftInch, delta, info + &quot;.WindowLeftInch&quot;);
            AssertHelper.AreEqual(expected.WindowTopCM, result.WindowTopCM, delta, info + &quot;.WindowTopCM&quot;);
            AssertHelper.AreEqual(expected.WindowTopInch, result.WindowTopInch, delta, info + &quot;.WindowTopInch&quot;);
            AssertHelper.AreEqual(expected.WindowWidthCM, result.WindowWidthCM, delta, info + &quot;.WindowWidthCM&quot;);
            AssertHelper.AreEqual(expected.WindowWidthInch, result.WindowWidthInch, delta, info + &quot;.WindowWidthInch&quot;);
            FormulaSettings fsExpected = expected.FormulaSettings;
            FormulaSettings fsResult = expected.FormulaSettings;
            AssertHelper.AreEqual(fsExpected.CalculateOnOpen, fsResult.CalculateOnOpen,
                info + &quot;.Settings.FormulaSettings.ReCalculateOnOpen&quot;);
            AssertHelper.AreEqual(fsExpected.CalculationMode, fsResult.CalculationMode,
                info + &quot;.Settings.FormulaSettings.CalculationMode&quot;);
            AssertHelper.AreEqual(fsExpected.EnableIterativeCalculation, fsResult.EnableIterativeCalculation,
                info + &quot;.Settings.FormulaSettings.EnableIterativeCalculation&quot;);
            AssertHelper.AreEqual(fsExpected.MaxChange, fsResult.MaxChange, delta,
                info + &quot;.Settings.FormulaSettings.MaxChange&quot;);
            AssertHelper.AreEqual(fsExpected.MaxIteration, fsResult.MaxIteration,
                info + &quot;.Settings.FormulaSettings.MaxIteration&quot;);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


