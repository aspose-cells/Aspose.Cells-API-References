---
title: "Worksheet.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Liest oder setzt den Namen des Arbeitsblatts."
type: docs
url: /de/net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Liest oder setzt den Namen des Arbeitsblatts.

```csharp
public string Name { get; set; }
```

### Hinweise

Die maximale Länge eines Blattnamens beträgt 31 Zeichen. Und Sie können nicht denselben Namen (Groß-/Kleinschreibung wird ignoriert) zwei Arbeitsblättern zuweisen. Zum Beispiel können Sie nicht "SheetName1" dem ersten Arbeitsblatt zuweisen und "SHEETNAME1" dem zweiten Arbeitsblatt zuweisen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und setzen Sie dessen Namen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Fügen Sie ein neues Arbeitsblatt mit einem bestimmten Namen hinzu
            Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
            
            // Geben Sie die Namen aller Arbeitsblätter aus
            Console.WriteLine("Worksheet Names:");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                Console.WriteLine(ws.Name);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


