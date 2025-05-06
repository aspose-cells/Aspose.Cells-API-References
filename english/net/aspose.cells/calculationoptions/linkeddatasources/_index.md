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
// Called: copts.LinkedDataSources = new Workbook[] { wb };
[Test]
        public void Property_LinkedDataSources()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[0, 0].PutValue(&quot;Col1&quot;);
            cells[0, 1].PutValue(&quot;Col2&quot;);
            cells[1, 0].PutValue(1);
            cells[1, 1].PutValue(2);
            cells[2, 0].PutValue(4);
            cells[2, 1].PutValue(8);
            Aspose.Cells.Tables.ListObjectCollection listObjects = sheet.ListObjects;
            listObjects.Add(&quot;A1&quot;, &quot;B3&quot;, true);
            wb.FileName = &quot;Book2.xlsx&quot;;
            CalculationOptions copts = new CalculationOptions();
            copts.LinkedDataSources = new Workbook[] { wb };
            copts.CustomEngine = new EngineN57494();

            wb = new Workbook();
            sheet = wb.Worksheets[0];
            string fml = &quot;=SUM(&apos;Book2.xlsx&apos;!Table1[#All])&quot;;
            object v = sheet.CalculateFormula(fml, copts);
            FormulaCaseUtil.AssertInt(15, v, fml);
            if (wb.Worksheets.ExternalLinks.Count &gt; 0)
            {
                Assert.Fail(&quot;0: Extra external links were created in calculation.&quot;);
            }
            fml = &quot;=SUM(INDIRECT(\&quot;&apos;Book2.xlsx&apos;!Table1[#All]\&quot;))&quot;;
            v = sheet.CalculateFormula(fml, copts);
            FormulaCaseUtil.AssertInt(15, v, fml);
            if (wb.Worksheets.ExternalLinks.Count &gt; 0)
            {
                Assert.Fail(&quot;1: Extra external links were created in calculation.&quot;);
            }
        }
```

### See Also

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


