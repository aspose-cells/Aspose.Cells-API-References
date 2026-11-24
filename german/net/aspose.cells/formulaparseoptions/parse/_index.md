---
title: "FormulaParseOptions.Parse"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaParseOptions-Eigenschaft. Gibt an, ob die angegebene Formel geparst werden soll. Standard ist true. Ist sie false, bleibt der Formel-String unverändert in der Zelle, bis der Benutzer andere Methoden zum Parsen aufruft oder geparste Formeldaten von anderen Vorgängen wie der Berechnung von Formeln benötigt werden."
type: docs
url: /de/net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

Ob die gegebene Formel geparst werden soll. Standard ist true. Wenn sie false ist, bleibt die Formelzeichenkette unverändert in der Zelle, bis der Benutzer andere Methoden zum Parsen aufruft oder geparste Formeldaten von anderen Vorgängen wie der Berechnung von Formeln benötigt werden.

```csharp
public bool Parse { get; set; }
```

### Beispiele

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

            // Formeln mit Parse=false festlegen (Formeln werden nicht sofort geparst)
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
            cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });

            // Formeln berechnen (Parsing erfolgt jetzt)
            wb.CalculateFormula();

            Console.WriteLine("B1 value: " + cells["B1"].Value);
            Console.WriteLine("B2 value: " + cells["B2"].Value);
        }
    }
}
```

### Siehe auch

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


