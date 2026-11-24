---
title: "DefaultStyleSettings.VerticalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DefaultStyleSettings-Eigenschaft. Gibt/Setzt den Standardwert für die vertikale Ausrichtung"
type: docs
url: /de/net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

Liest/Setzt den Standardwert für die vertikale Ausrichtung

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Standard‑vertikale Ausrichtung auf Unten setzen
            LoadOptions options = new LoadOptions();
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["B1"].PutValue("Sample Text 2");
            worksheet.Cells["C1"].PutValue("Sample Text 3");

            // Überprüfen, dass die vertikale Ausrichtung auf alle Zellen angewendet wird
            foreach (Cell cell in worksheet.Cells)
            {
                Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


