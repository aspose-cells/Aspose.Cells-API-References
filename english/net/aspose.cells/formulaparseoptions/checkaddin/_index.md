---
title: FormulaParseOptions.CheckAddIn
second_title: Aspose.Cells for .NET API Reference
description: FormulaParseOptions property. Whether check addins in existing external links of current workbook for user defined function without external link. Default is trueif user defined function matches one addin in existing external links then take it as the addin
type: docs
url: /net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).

```csharp
public bool CheckAddIn { get; set; }
```

### Examples

```csharp
// Called: sheet.Cells[0, 0].SetFormula(&amp;quot;=dsfun(B1)&amp;quot;, new FormulaParseOptions() { CheckAddIn = false }, null);
[Test]
        public void Property_CheckAddIn()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells[0, 0].Formula = &quot;&apos;externalDS.xlam&apos;!dsfun(B1)&quot;;
            Assert.AreEqual(&quot;=externalDS.xlam!dsfun(B1)&quot;, sheet.Cells[0, 0].Formula);
            sheet.Cells[0, 0].SetFormula(&quot;=dsfun(B1)&quot;, new FormulaParseOptions() { CheckAddIn = false }, null);
            Assert.AreEqual(&quot;=dsfun(B1)&quot;, sheet.Cells[0, 0].Formula);

            sheet.Cells[0, 0].Formula = &quot;&apos;externalDS.xlam&apos;!dsfun(B1)&quot;;
            Assert.AreEqual(&quot;=externalDS.xlam!dsfun(B1)&quot;, sheet.Cells[0, 0].Formula);
            wb = new Workbook();
            wb.Worksheets[0].Cells[0, 0].Formula = &quot;&apos;externalDS.xlam&apos;!dsfunnew(C1)&quot;;
            wb.Worksheets[0].Copy(sheet);
            Assert.AreEqual(&quot;=externalDS.xlam!dsfun(B1)&quot;, wb.Worksheets[0].Cells[0, 0].Formula);
        }
```

### See Also

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


