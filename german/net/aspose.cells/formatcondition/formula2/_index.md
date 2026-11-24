---
title: "FormatCondition.Formula2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Ruft den Wert oder Ausdruck ab und legt ihn fest, der mit der bedingten Formatierung verknüpft ist."
type: docs
url: /de/net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Liest und setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist.

```csharp
public string Formula2 { get; set; }
```

### Hinweise

Bitte fügen Sie alle Bereiche hinzu, bevor Sie die Formel festlegen. Beim Festlegen der Formel für diese Bedingung wird ein Eingabewert, der mit '=' beginnt, als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=' beginnen, kann der Benutzer die Formel im Format "=\"=...\"" eingeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula2Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bedingte Formatierung hinzufügen
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[index];
            
            // Definieren Sie den Zellbereich
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            
            // Fügen Sie eine Formatbedingung mit Formula2 hinzu
            formatConditions.Add(area, 
                FormatConditionType.CellValue, 
                OperatorType.Between, 
                "=\"abc def\"", 
                "=\"a\"&\"b\"");

            // Rufen Sie die Formatbedingung ab
            FormatCondition formatCondition = formatConditions[0];

            // Geben Sie die Formeln aus
            Console.WriteLine("Formula1: " + formatCondition.Formula1);
            Console.WriteLine("Formula2: " + formatCondition.Formula2);

            // Speichere die Arbeitsmappe
            workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


