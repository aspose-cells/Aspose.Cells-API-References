---
title: WorkbookSettings.EnableMacros
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Enable macros
type: docs
url: /net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

Enable macros;

```csharp
public bool EnableMacros { get; set; }
```

### Remarks

Now it only works when copying a worksheet to other worksheet in a workbook.

### Examples

```csharp
// Called: wb.Settings.EnableMacros = false;
public void WorkbookSettings_Property_EnableMacros()
{
    string filePath = Constants.PivotTableSourcePath + @"NET42322_";
    Workbook wb = new Workbook(filePath + "Model.xlsm");
    wb.Settings.CheckCompatibility = false;
    wb.Settings.CheckExcelRestriction = false;
    wb.Settings.EnableMacros = false;

    foreach (Worksheet sheet in wb.Worksheets)
    {
        if (sheet.Name.Equals("dati"))
        {
            sheet.Cells.DeleteRows(5, sheet.Cells.Rows.Count - 1);
        }
    }

    foreach (Worksheet w in wb.Worksheets)
    {
        foreach (PivotTable pv in w.PivotTables)
        {
            pv.PreserveFormatting = true;
            pv.RefreshData();
            pv.CalculateData();
        }
        if (
            (w.Name.ToLower() == "param_filtri")
            ||
            (w.Name.ToLower() == "parametri_selez")
            ||
            (w.Name.ToLower() == "calcoli_addett_giorni")
           )
        {
            w.VisibilityType = VisibilityType.VeryHidden;
        }
    }

    wb.Save(Constants.PIVOT_CHECK_FILE_PATH + "example.xlsx");
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


