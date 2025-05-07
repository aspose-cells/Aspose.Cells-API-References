---
title: WorkbookSettings.SheetTabBarWidth
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Width of worksheet tab bar in 1/1000 of window width
type: docs
url: /net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Width of worksheet tab bar (in 1/1000 of window width).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(book.Settings.IsHidden + "," + book.Settings.SheetTabBarWidth);
[Test]
        public void Property_SheetTabBarWidth()
        {
            Workbook book = null;
            Console.WriteLine("Property_SheetTabBarWidth()");
            string binfn = path + "TEST_BookOptions.xlsx";
            book = new Workbook(binfn);
            WorkbookSettings settings1 = book.Settings;
            book = Util.ReSave(book, SaveFormat.Xlsx);
            WorkbookSettings settings2 = book.Settings;
            Assert.AreEqual(settings1.ShowTabs, settings2.ShowTabs);
            Assert.AreEqual(settings1.FormulaSettings.CalculationMode, settings2.FormulaSettings.CalculationMode);
            Assert.AreEqual(settings1.FormulaSettings.PrecisionAsDisplayed, settings2.FormulaSettings.PrecisionAsDisplayed);
            Assert.AreEqual(settings1.FormulaSettings.CalculateOnSave, settings2.FormulaSettings.CalculateOnSave);

            string ssinfn = path + "TEST_SheetsOptions.xlsx";
            string ssoutfn = Constants.destPath + "TEST_SheetsOptions_out.xlsx";
            book = new Workbook(ssinfn);
            Console.WriteLine(book.Settings.IsHidden + "," + book.Settings.SheetTabBarWidth);
            book.Save(ssoutfn);
            book= new Workbook(ssoutfn);
            Console.WriteLine(book.Settings.IsHidden + "," + book.Settings.SheetTabBarWidth);

            string sinfn = path + "TEST_SheetOptions.xlsx";
            string soutfn = Constants.destPath + "TEST_SheetOptions_out.xlsx";
            book = new Workbook(sinfn);
            book.Save(soutfn);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


