---
title: FormulaSettings.PrecisionAsDisplayed
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Whether the precision of calculated result be set as they are displayed while calculating formulas
type: docs
url: /net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Whether the precision of calculated result be set as they are displayed while calculating formulas

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(settings1.FormulaSettings.PrecisionAsDisplayed, settings2.FormulaSettings.PrecisionAsDisplayed);
[Test]
        public void Property_PrecisionAsDisplayed()
        {
            Workbook book = null;
            Console.WriteLine(&quot;Property_PrecisionAsDisplayed()&quot;);
            string binfn = path + &quot;TEST_BookOptions.xlsx&quot;;
            book = new Workbook(binfn);
            WorkbookSettings settings1 = book.Settings;
            book = Util.ReSave(book, SaveFormat.Xlsx);
            WorkbookSettings settings2 = book.Settings;
            Assert.AreEqual(settings1.ShowTabs, settings2.ShowTabs);
            Assert.AreEqual(settings1.FormulaSettings.CalculationMode, settings2.FormulaSettings.CalculationMode);
            Assert.AreEqual(settings1.FormulaSettings.PrecisionAsDisplayed, settings2.FormulaSettings.PrecisionAsDisplayed);
            Assert.AreEqual(settings1.FormulaSettings.CalculateOnSave, settings2.FormulaSettings.CalculateOnSave);

            string ssinfn = path + &quot;TEST_SheetsOptions.xlsx&quot;;
            string ssoutfn = Constants.destPath + &quot;TEST_SheetsOptions_out.xlsx&quot;;
            book = new Workbook(ssinfn);
            Console.WriteLine(book.Settings.IsHidden + &quot;,&quot; + book.Settings.SheetTabBarWidth);
            book.Save(ssoutfn);
            book= new Workbook(ssoutfn);
            Console.WriteLine(book.Settings.IsHidden + &quot;,&quot; + book.Settings.SheetTabBarWidth);

            string sinfn = path + &quot;TEST_SheetOptions.xlsx&quot;;
            string soutfn = Constants.destPath + &quot;TEST_SheetOptions_out.xlsx&quot;;
            book = new Workbook(sinfn);
            book.Save(soutfn);
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


