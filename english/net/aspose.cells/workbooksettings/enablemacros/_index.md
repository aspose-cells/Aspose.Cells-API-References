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
[Test]
        public void Property_EnableMacros()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET42322_&quot;;
            Workbook wb = new Workbook(filePath + &quot;Model.xlsm&quot;);
            wb.Settings.CheckCompatibility = false;
            wb.Settings.CheckExcelRestriction = false;
            wb.Settings.EnableMacros = false;

            foreach (Worksheet sheet in wb.Worksheets)
            {
                if (sheet.Name.Equals(&quot;dati&quot;))
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
                    (w.Name.ToLower() == &quot;param_filtri&quot;)
                    ||
                    (w.Name.ToLower() == &quot;parametri_selez&quot;)
                    ||
                    (w.Name.ToLower() == &quot;calcoli_addett_giorni&quot;)
                   )
                {
                    w.VisibilityType = VisibilityType.VeryHidden;
                }
            }

            wb.Save(Constants.PIVOT_CHECK_FILE_PATH + &quot;NET42322.xlsx&quot;);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


