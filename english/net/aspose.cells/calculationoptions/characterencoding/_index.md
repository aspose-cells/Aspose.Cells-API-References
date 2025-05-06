---
title: CalculationOptions.CharacterEncoding
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR CODE the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result
type: docs
url: /net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### Examples

```csharp
// Called: copts.CharacterEncoding = Encoding.GetEncoding(&amp;quot;iso-2022-jp&amp;quot;);
[Test]
        public void Property_CharacterEncoding()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            wb.Settings.Region = CountryCode.Japan;
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding(&quot;iso-2022-jp&quot;);
            string fml = &quot;=TRIM(1)&quot;;
            Assert.AreEqual(&quot;1&quot;, sheet.CalculateFormula(fml, copts));
        }
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


