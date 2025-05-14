---
title: Enum SlicerStyleType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Slicers.SlicerStyleType enum. Specify the style of slicer view
type: docs
url: /net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Specify the style of slicer view

```csharp
public enum SlicerStyleType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | built-in light style one |
| SlicerStyleLight2 | `1` | built-in light style two |
| SlicerStyleLight3 | `2` | built-in light style three |
| SlicerStyleLight4 | `3` | built-in light style four |
| SlicerStyleLight5 | `4` | built-in light style five |
| SlicerStyleLight6 | `5` | built-in light style six |
| SlicerStyleOther1 | `6` | built-in style other one |
| SlicerStyleOther2 | `7` | built-in style other two |
| SlicerStyleDark1 | `8` | built-in dark style one |
| SlicerStyleDark2 | `9` | built-in dark style tow |
| SlicerStyleDark3 | `10` | built-in dark style three |
| SlicerStyleDark4 | `11` | built-in dark style four |
| SlicerStyleDark5 | `12` | built-in dark style five |
| SlicerStyleDark6 | `13` | built-in dark style six |
| Custom | `14` | user-defined style, unsupported for now |

### Examples

```csharp
// Called: slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
public void Slicers_Type_SlicerStyleType()
{
    string filePath = Constants.PivotTableSourcePath + @"NET44455_";

    Workbook wb = null;
    wb = new Workbook(filePath + "issue.xlsx");
    wb.Save(CreateFolder(filePath) + "issue_out.pdf");

    wb = new Workbook(filePath + "aaa.xlsx");
    wb.Save(CreateFolder(filePath) + "aaa_out.pdf");
    wb = new Workbook(filePath + "bbb.xlsx");
    wb.Settings.GlobalizationSettings.PivotSettings = new CustomGlobal44455();
    wb.Save(CreateFolder(filePath) + "bbb_out.pdf");

    #region read and write for xlsb and xlsx
    wb = new Workbook(filePath + "slicer.xlsx");
    wb.Save(CreateFolder(filePath) + "slicer_out.xlsx");
    wb = new Workbook(filePath + "slicer.xlsb");
    wb.Save(CreateFolder(filePath) + "slicer_out.xlsb");
    #endregion

    #region conversion between xlsb and xlsx
    wb = new Workbook(filePath + "slicer.xlsx");
    wb.Save(CreateFolder(filePath) + "slicer_out1.xlsx");
    wb.Save(CreateFolder(filePath) + "slicer_out1.xlsb");//ok
    wb.Save(Constants.PivotTableDestPath + @"example.html");
    wb = new Workbook(filePath + "slicer.xlsb");
    wb.Save(CreateFolder(filePath) + "slicer_out2.xlsx");//ok
    wb.Save(CreateFolder(filePath) + "slicer_out2.xlsb");
    #endregion


    #region create slicer
    wb = new Workbook(filePath + "a.xlsx");
    Worksheet sheet = wb.Worksheets[0];
    PivotTable pivot = sheet.PivotTables[0];
    int index = sheet.Slicers.Add(pivot, "A10", pivot.BaseFields[0]);
    Slicer slicer = sheet.Slicers[index];
    slicer.NumberOfColumns = 2;
    slicer.StyleType = SlicerStyleType.SlicerStyleDark1;


    wb.Save(CreateFolder(filePath) + "a_createSlicer.xlsx");
    wb.Save(CreateFolder(filePath) + "a_createSlicer.xlsb");
    wb.Save(CreateFolder(filePath) + "a_createSlicer.pdf");

    SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
    int itemCount = items.Count;
    for (int i = 0; i < itemCount; i++)
    {
        SlicerCacheItem item = items[i];
        //only select partial items 
        if (i % 2 == 0)
        {
            item.Selected = false;
        }
    }
    slicer.Refresh();

    wb.Save(CreateFolder(filePath) + "a_updateSlicer.xlsx");
    wb.Save(CreateFolder(filePath) + "a_updateSlicer.xlsb");
    wb.Save(CreateFolder(filePath) + "a_updateSlicer.pdf");

    sheet.Slicers.Remove(slicer);
    wb.Save(CreateFolder(filePath) + "a_removeSlicer.xlsx");
    wb.Save(CreateFolder(filePath) + "a_removeSlicer.xlsb");
    wb.Save(CreateFolder(filePath) + "a_removeSlicer.pdf");
    #endregion

    #region chart issue
    wb = new Workbook(filePath + "chart.xlsx");
    wb.Save(CreateFolder(filePath) + "chart_toXls.xls");
    #endregion
}
```

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


