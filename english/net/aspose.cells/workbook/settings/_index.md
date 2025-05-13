---
title: Workbook.Settings
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Represents the workbook settings
type: docs
url: /net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Represents the workbook settings.

```csharp
public WorkbookSettings Settings { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Settings.FormulaSettings.EnableIterativeCalculation);
// Zhao Xilong Issue
public void Workbook_Property_Settings()
{
    Console.WriteLine("Workbook_Property_Settings()");
    string infn = path + @"example.xlsm";
    string outfn = Constants.destPath + @"example.xlsm";

    Workbook workbook = new Workbook(infn);
    Assert.IsTrue(workbook.Settings.FormulaSettings.EnableIterativeCalculation);
    Assert.AreEqual(30, workbook.Settings.FormulaSettings.MaxIteration);
    Assert.AreEqual(0.1, workbook.Settings.FormulaSettings.MaxChange);
    workbook.Save(outfn);
}
```

### See Also

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


