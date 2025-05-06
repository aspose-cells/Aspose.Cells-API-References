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
// Called: wb.Settings.Region = CountryCode.USA;
[Test]
        public void Property_Region()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            StringBuilder sbV = new StringBuilder();
            StringBuilder sbL = new StringBuilder();
            AppendSpaces(sbV, sbL);
            sbV.Append(&quot;ABC&quot;);
            sbL.Append(&quot;ABC&quot;);
            string literal = sbL.ToString();
            cells[0, 1].PutValue(sbV.ToString());
            cells[0, 2].PutValue(&quot;ABC&quot;);
            cells[0, 3].PutValue(1000);
            Cell cell = cells[0, 0];
            cell.Formula = &quot;=VLOOKUP(TRIM(B1),C1:D1,2,false)&quot;;
            wb.Settings.Region = CountryCode.USA;
            wb.CalculateFormula();
            Assert.AreEqual(&quot;#N/A&quot;, cell.StringValue, &quot;TRIM for USA: &quot; + literal);
            wb.Settings.Region = CountryCode.China;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;1000&quot;, cell.StringValue, &quot;TRIM for China: &quot; + literal);
            wb.Settings.Region = CountryCode.Japan;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;1000&quot;, cell.StringValue, &quot;TRIM for Japan: &quot; + literal);

            cell.Formula = &quot;=TRIM(\&quot;\u3000\u3000A\u0020\u3000BC\&quot;)&quot;;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;A BC&quot;, cell.StringValue, &quot;TRIM for continuous white spaces start with &apos; &apos;&quot;);
            cell.Formula = &quot;=TRIM(\&quot;\u3000\u3000A\u3000\u0020BC\&quot;)&quot;;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;A\u3000BC&quot;, cell.StringValue, &quot;TRIM for continuous white spaces start with &apos;　&apos;&quot;);
            sbV.Length = sbV.Length - 2;
            sbL.Length = sbL.Length - 2;
            sbV.Insert(0, &quot;=TRIM(\&quot;&quot;);
            sbL.Insert(0, &quot;=TRIM(\&quot;&quot;);
            int pos = sbV.Length;
            AppendSpaces(sbV, sbL);
            sbV.Append(&quot;BC\&quot;)&quot;);
            sbL.Append(&quot;BC\&quot;)&quot;);
            cell.Formula = sbV.ToString();
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;A&quot; + sbV[pos] + &quot;BC&quot;, cell.StringValue, &quot;TRIM for continuous white spaces: &quot; + sbL.ToString());
        }
```

### See Also

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


