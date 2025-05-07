---
title: WorkbookSettings.Region
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets the regional settings for workbook
type: docs
url: /net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Gets or sets the regional settings for workbook.

```csharp
public CountryCode Region { get; set; }
```

### Remarks

1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

### Examples

```csharp
// Called: wb.Settings.Region = CountryCode.Norway;
[Test]
        public void Property_Region()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Finland;
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            cell.PutValue(0.5);
            Style style = cell.GetStyle();
            style.Number = 9;
            cell.SetStyle(style);
            Assert.AreEqual("50 %", cell.StringValue, "Finland-9");
            style.Number = 10;
            cell.SetStyle(style);
            Assert.AreEqual("50,00 %", cell.StringValue, "Finland-9");
            wb.Settings.Region = CountryCode.Norway;
            for (int i = 7; i < 11; i++)
            {
                style.Number = i;
                cell.SetStyle(style);
                Assert.IsTrue(cell.StringValue.IndexOf(' ') > 0, "Norway-" + i);
            }
        }
```

### See Also

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


