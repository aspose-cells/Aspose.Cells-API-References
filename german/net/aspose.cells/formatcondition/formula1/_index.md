---
title: "FormatCondition.Formula1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Ruft den Wert oder Ausdruck ab und legt ihn fest, der mit der bedingten Formatierung verknüpft ist."
type: docs
url: /de/net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

Liest und setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist.

```csharp
public string Formula1 { get; set; }
```

### Hinweise

Bitte fügen Sie alle Bereiche hinzu, bevor Sie die Formel festlegen. Beim Festlegen der Formel für diese Bedingung wird ein Eingabewert, der mit '=' beginnt, als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer die Formel im Format "=\"=...\"" eingeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula1Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["E1"].PutValue(50);
            
            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Legen Sie den Bereich und den Bedingungstyp fest
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
            
            // Greifen Sie auf die Formula1-Eigenschaft zu und zeigen Sie sie an
            FormatCondition fc = fcc[0];
            Console.WriteLine("Formula1: " + fc.Formula1);
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


