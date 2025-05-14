---
title: WorkbookSettings.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether this workbook is hidden
type: docs
url: /net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Indicates whether this workbook is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(book.Settings.IsHidden + "," + book.Settings.SheetTabBarWidth);
public void WorkbookSettings_Property_IsHidden()
{
    Workbook book = null;
    Console.WriteLine("WorkbookSettings_Property_IsHidden()");
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


