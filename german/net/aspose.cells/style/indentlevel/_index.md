---
title: "Style.IndentLevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt das Einrückungsniveau für die Zelle oder den Bereich an. Kann nur ein ganzzahliger Wert von 0 bis 250 sein."
type: docs
url: /de/net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Stellt die Einzugsebene für die Zelle oder den Bereich dar. Kann nur ein ganzzahliger Wert von 0 bis 250 sein.

```csharp
public int IndentLevel { get; set; }
```

### Hinweise

Wenn die horizontale Ausrichtung des Textes auf einen anderen Wert als links oder rechts gesetzt ist, wird das Einrückungsniveau auf Null zurückgesetzt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIndentLevelDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Legen Sie unterschiedliche Einrückungsniveaus für Zellen fest.
            for (int i = 0; i < 16; i++)
            {
                Cell cell = cells[i, 0];
                Style style = cell.GetStyle();
                style.IndentLevel = i;
                style.HorizontalAlignment = TextAlignmentType.Left;
                cell.SetStyle(style);
                cell.PutValue($"Indent Level {i}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("IndentLevelDemo.xlsx");
            Console.WriteLine("Workbook saved with different indent levels.");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


