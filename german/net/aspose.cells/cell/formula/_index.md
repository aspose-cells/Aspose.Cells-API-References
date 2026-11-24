---
title: "Cell.Formula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Liest oder setzt die Formel der Zelle"
type: docs
url: /de/net/aspose.cells/cell/formula/
---
## Cell.Formula property

Liest oder setzt die Formel der [`Cell`](../).

```csharp
public string Formula { get; set; }
```

### Hinweise

Eine Formelkette beginnt immer mit einem Gleichheitszeichen (=). Und bitte immer das Komma (,) als Parametertrennzeichen verwenden, zum Beispiel "=SUM(A1, E1, H2)".

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Werte in Zellen festlegen, die in der Formel verwendet werden
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A1"].PutValue(100);

            // Formel in Zelle B6 festlegen
            worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";

            // Formel berechnen
            workbook.CalculateFormula();

            // Ergebnis anzeigen
            Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


