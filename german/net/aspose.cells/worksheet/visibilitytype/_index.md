---
title: "Worksheet.VisibilityType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt den Sichtbarkeitszustand dieses Blatts an"
type: docs
url: /de/net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

Gibt den Sichtbarkeitszustand für dieses Blatt an.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVisibilityTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblätter hinzufügen
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Unterschiedliche Sichtbarkeitstypen für jedes Arbeitsblatt festlegen
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;

            // Speichere die Arbeitsmappe
            string outputPath = "output_visibility.xlsx";
            workbook.Save(outputPath);

            // Laden Sie die Arbeitsmappe erneut, um die Sichtbarkeitseinstellungen zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Sichtbarkeitstypen ausgeben
            Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
            Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
            Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
        }
    }
}
```

### Siehe auch

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


