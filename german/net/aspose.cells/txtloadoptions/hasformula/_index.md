---
title: "TxtLoadOptions.HasFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions-Eigenschaft. Gibt an, ob der Text eine Formel ist, wenn er beginnt mit"
type: docs
url: /de/net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt.

```csharp
public bool HasFormula { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Erstelle Text-Ladeoptionen und aktiviere die Formelauswertung
            TxtLoadOptions options = new TxtLoadOptions();
            options.HasFormula = true;
            options.SeparatorString = "|";

            // Lade die Arbeitsmappe mit Formeln in der Textdatei
            Workbook workbook = new Workbook("example.csv", options);
            
            // Greife auf eine Zelle mit Formel zu und zeige sie an
            Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
            
            // Speichere die Arbeitsmappe
            workbook.Save("example_output.xlsx");
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


