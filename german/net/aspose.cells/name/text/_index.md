---
title: "Name.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Eigenschaft. Gibt den Namens-Text des Objekts zurück"
type: docs
url: /de/net/aspose.cells/name/text/
---
## Name.Text property

Liest den Namens-Text des Objekts.

```csharp
public string Text { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblatt hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Benannten Bereich erstellen
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Setzen und Anzeigen der Text-Eigenschaft
            namedRange.Text = "MyCustomName";
            Console.WriteLine("Named range text: " + namedRange.Text);
            
            // Speichere die Arbeitsmappe
            workbook.Save("NamedRangeExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


