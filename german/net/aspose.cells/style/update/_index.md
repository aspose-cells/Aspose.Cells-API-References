---
title: "Style.Update"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Wendet den benannten Stil auf die Stile der Zellen an, die diesen benannten Stil verwenden. Es funktioniert wie das Klicken auf die OK-Schaltfläche, nachdem du den Stil bearbeitet hast. Gilt nur für benannte Stile"
type: docs
url: /de/net/aspose.cells/style/update/
---
## Style.Update method

Wendet den benannten Stil auf die Stile der Zellen an, die diesen benannten Stil verwenden. Es funktioniert wie das Klicken auf die Schaltfläche \"ok\" nachdem Sie den Stil bearbeitet haben. Gilt nur für benannte Stile.

```csharp
public void Update()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodUpdateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen Stil
            Style style = workbook.CreateStyle();
            style.Number = 3; // Set to Percent format
            
            // Den Stil auf Zelle A1 anwenden
            worksheet.Cells["A1"].SetStyle(style);
            
            // Stil ändern
            style.Number = 4; // Change to Currency format
            
            // Aktualisiere die Stiländerungen
            style.Update();
            
            // Überprüfen Sie, ob der Stil aktualisiert wurde
            Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


