---
title: CalculationOptions.LinkedDataSources
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Specifies the data sources for external links used in formulas
type: docs
url: /net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Specifies the data sources for external links used in formulas.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Remarks

Like [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). The match of those workbooks with external links is determined by [`FileName`](../../workbook/filename/) and [`DataSource`](../../externallink/datasource/). So please make sure [`FileName`](../../workbook/filename/) has been specified with the proper value(generally it should be same with corresponding [`DataSource`](../../externallink/datasource/)) for every workbook so they can be linked as expected.

### Examples

```csharp
// Called: cell.Calculate(new CalculationOptions() { LinkedDataSources = new Workbook[] { wbExt } });
[Test]
        public void Property_LinkedDataSources()
        {
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells[1, 0].PutValue(3);
            wbExt.Worksheets.Add("Sheet2").Cells[1, 0].PutValue(4);
            wbExt.Worksheets.Names.Add("Sheet1!MyNumber1");
            wbExt.Worksheets.Names[0].RefersTo = "=Sheet1!$A$2";
            wbExt.Worksheets.Names.Add("Sheet2!MyNumber2");
            wbExt.Worksheets.Names[1].RefersTo = "=Sheet2!$A$2";
            wbExt.Worksheets.Names.Add("MyNumber3");
            wbExt.Worksheets.Names[2].RefersTo = "=Sheet1!$A$2";

            wbExt.FileName = "B.xlsx";
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            //to reproduce the original bug, B.XLSX cannot exist in formula as direct external reference
            cell.Formula = "=INDIRECT(\"[B.XLSX]Sheet1!$A$2\")";
            cell.Calculate(new CalculationOptions() { LinkedDataSources = new Workbook[] { wbExt } });
            AssertHelper.Equals(3, cell, "INDIRECT to address in external link with empty ExternalLinks");
            cell.Formula = "=INDIRECT(\"[B.XLSX]Sheet1!MyNumber1\")";
            cell.Calculate(new CalculationOptions() { LinkedDataSources = new Workbook[] { wbExt } });
            AssertHelper.Equals(3, cell, "INDIRECT to defined name in external link with empty ExternalLinks");
            cell.Formula = "=INDIRECT(\"[B.XLSX]!MyNumber3\")";
            cell.Calculate(new CalculationOptions() { LinkedDataSources = new Workbook[] { wbExt } });
            AssertHelper.Equals(3, cell, "INDIRECT to defined global name in external link with empty ExternalLinks");
            Assert.AreEqual(0, wb.Worksheets.ExternalLinks.Count, "Count of workbook's external link");

            //add external link
            cell.Formula = "=[B.XLSX]Sheet2!$A$2";
            cell.Formula = "=[B.XLSX]Sheet2!MyNumber2";
            cell.Formula = "=INDIRECT(\"[B.XLSX]Sheet1!$A$2\")";
            cell.Calculate(new CalculationOptions() { LinkedDataSources = new Workbook[] { wbExt } });
            AssertHelper.Equals(3, cell, "INDIRECT to address in external link with another sheet");
            cell.Formula = "=INDIRECT(\"[B.XLSX]Sheet2!MyNumber2\")";
            cell.Calculate(new CalculationOptions() { LinkedDataSources = new Workbook[] { wbExt } });
            AssertHelper.Equals(4, cell, "INDIRECT to existing defined name in external link");
            cell.Formula = "=INDIRECT(\"[B.XLSX]Sheet1!MyNumber1\")";
            cell.Calculate(new CalculationOptions() { LinkedDataSources = new Workbook[] { wbExt } });
            AssertHelper.Equals(3, cell, "INDIRECT to non-existing defined name in external link");
            cell.Formula = "=INDIRECT(\"[B.XLSX]Sheet2!MyNumber1\")";
            cell.Calculate(new CalculationOptions() { LinkedDataSources = new Workbook[] { wbExt } });
            Assert.AreEqual("#REF!", cell.StringValue, "INDIRECT to non-defined name of external link");
            MemoryStream ms = Util.SaveAsBuffer(wb, SaveFormat.Xlsx);
            if (!ManualFileUtil.ManualCheckStringInZip(ms, "xl/externalLinks/externalLink1.xml",
                new string[] { "sheetName val=\"Sheet1\"", "definedName name=\"MyNumber1\"", }, false))
            {
                Assert.Fail("Sheet1 and MyNumber1 should not exist in saved workbook after calculation");
            }
        }
```

### See Also

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


