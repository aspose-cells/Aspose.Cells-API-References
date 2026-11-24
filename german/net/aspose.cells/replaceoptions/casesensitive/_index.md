---
title: "ReplaceOptions.CaseSensitive"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReplaceOptions-Eigenschaft. Gibt an, ob die gesuchte Zeichenfolge Groß-/Kleinschreibung beachtet"
type: docs
url: /de/net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Gibt an, ob die gesuchte Zeichenfolge Groß‑ und Kleinschreibung beachtet.

```csharp
public bool CaseSensitive { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Ersetzungsoptionen mit CaseSensitive = false erstellen
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            
            // Alle Groß-/Kleinschreibungsvarianten von "apple" durch "orange" ersetzen
            workbook.Replace("apple", "orange", options);

            // Ergebnisse ausgeben
            Console.WriteLine("After replacement (CaseSensitive = false):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Daten zurücksetzen
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Ändern zu CaseSensitive = true
            options.CaseSensitive = true;
            workbook.Replace("apple", "orange", options);

            // Ergebnisse ausgeben
            Console.WriteLine("\nAfter replacement (CaseSensitive = true):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Siehe auch

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


