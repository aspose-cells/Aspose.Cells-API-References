---
title: CalculationOptions.IgnoreError
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function external links etc. The default value is true
type: docs
url: /net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

```csharp
public bool IgnoreError { get; set; }
```

### Examples

```csharp
// Called: copts.IgnoreError = false;
[Test]
        public void Property_IgnoreError()
        {
            Workbook wb = new Workbook();
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add(&quot;mytestname&quot;)];
            string rs = &quot;$A$10:$A$13,$B$10:$D$10,$B$12:$D$14&quot;;
            n.RefersTo = rs;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.Formula = &quot;=MULTIREF(mytestname)&quot;;
            CalculationOptions copts = new CalculationOptions();
            copts.IgnoreError = false;
            copts.CustomEngine = new CustomEngineSimple();
            wb.CalculateFormula(copts);
            Assert.AreEqual(rs, cell.Value, &quot;CalculatedValue for multiple references&quot;);
        }
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


