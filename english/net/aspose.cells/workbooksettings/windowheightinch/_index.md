---
title: WorkbookSettings.WindowHeightInch
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. The height of the window in unit of inch
type: docs
url: /net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

The height of the window, in unit of inch.

```csharp
public double WindowHeightInch { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(expected.WindowHeightInch, result.WindowHeightInch, delta, info + ".WindowHeightInch");
private static void Property_WindowHeightInch(WorkbookSettings expected, WorkbookSettings result, string info)
        {
            AssertHelper.AreEqual(expected.Date1904, result.Date1904, info + ".Settings.Date1904");

            AssertHelper.AreEqual(expected.DisplayDrawingObjects, result.DisplayDrawingObjects, info + ".Settings.DisplayDrawingObjects");

            AssertHelper.AreEqual(expected.IsHScrollBarVisible, result.IsHScrollBarVisible, info + ".Settings.IsHScrollBarVisible");
            AssertHelper.AreEqual(expected.IsProtected, result.IsProtected, info + ".Settings.IsProtected");
            AssertHelper.AreEqual(expected.IsVScrollBarVisible, result.IsVScrollBarVisible, info + ".Settings.IsVScrollBarVisible");
            AssertHelper.AreEqual(expected.LanguageCode, result.LanguageCode, info + ".Settings.LanguageCode");
            AssertHelper.AreEqual(expected.Password, result.Password, info + ".Settings.Password");
            AssertHelper.AreEqual(expected.Region, result.Region, info + ".Settings.Region");
            AssertHelper.AreEqual(expected.Shared, result.Shared, info + ".Settings.Shared");
            AssertHelper.AreEqual(expected.ShowTabs, result.ShowTabs, info + ".Settings.ShowTabs");
            AssertHelper.AreEqual(expected.DisplayDrawingObjects, result.DisplayDrawingObjects, info + ".Settings.DisplayDrawingObjects");
            AssertHelper.AreEqual(expected.SheetTabBarWidth, result.SheetTabBarWidth, info + ".SheetTabBarWidth");
            AssertHelper.AreEqual(expected.WindowHeightCM, result.WindowHeightCM, delta, info + ".WindowHeightCM");
            AssertHelper.AreEqual(expected.WindowHeightInch, result.WindowHeightInch, delta, info + ".WindowHeightInch");
            AssertHelper.AreEqual(expected.WindowLeftCM, result.WindowLeftCM, delta, info + ".WindowLeftCM");
            AssertHelper.AreEqual(expected.WindowLeftInch, result.WindowLeftInch, delta, info + ".WindowLeftInch");
            AssertHelper.AreEqual(expected.WindowTopCM, result.WindowTopCM, delta, info + ".WindowTopCM");
            AssertHelper.AreEqual(expected.WindowTopInch, result.WindowTopInch, delta, info + ".WindowTopInch");
            AssertHelper.AreEqual(expected.WindowWidthCM, result.WindowWidthCM, delta, info + ".WindowWidthCM");
            AssertHelper.AreEqual(expected.WindowWidthInch, result.WindowWidthInch, delta, info + ".WindowWidthInch");
            FormulaSettings fsExpected = expected.FormulaSettings;
            FormulaSettings fsResult = expected.FormulaSettings;
            AssertHelper.AreEqual(fsExpected.CalculateOnOpen, fsResult.CalculateOnOpen,
                info + ".Settings.FormulaSettings.ReCalculateOnOpen");
            AssertHelper.AreEqual(fsExpected.CalculationMode, fsResult.CalculationMode,
                info + ".Settings.FormulaSettings.CalculationMode");
            AssertHelper.AreEqual(fsExpected.EnableIterativeCalculation, fsResult.EnableIterativeCalculation,
                info + ".Settings.FormulaSettings.EnableIterativeCalculation");
            AssertHelper.AreEqual(fsExpected.MaxChange, fsResult.MaxChange, delta,
                info + ".Settings.FormulaSettings.MaxChange");
            AssertHelper.AreEqual(fsExpected.MaxIteration, fsResult.MaxIteration,
                info + ".Settings.FormulaSettings.MaxIteration");
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


