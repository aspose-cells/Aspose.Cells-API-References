---
title: "FormulaParseOptions.Parse"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaParseOptions egenskap. Anger om given formel ska parsas. Standard är sant. Om den är falsk kommer den givna formelsträngen att behållas oförändrad för cellen tills användaren anropar andra metoder för att parsa den eller parsad formeldatan krävs av andra operationer såsom beräkning av formler"
type: docs
url: /sv/net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

Om given formel ska analyseras. Standard är true. Om den är false, behålls formelsträngen oförändrad i cellen tills användaren anropar andra metoder för att analysera den eller analyserad formeldatat behövs för andra operationer såsom beräkning av formler.

```csharp
public bool Parse { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyParseDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ange formler med Parse=false (formler kommer inte att parsas omedelbart)
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
            cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });

            // Beräkna formler (parsning kommer att ske nu)
            wb.CalculateFormula();

            Console.WriteLine("B1 value: " + cells["B1"].Value);
            Console.WriteLine("B2 value: " + cells["B2"].Value);
        }
    }
}
```

### Se även

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


