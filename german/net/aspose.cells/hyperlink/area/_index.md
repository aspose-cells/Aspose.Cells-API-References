---
title: "Hyperlink.Area"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Hyperlink-Eigenschaft. Gibt den Bereich des Hyperlinks zurück"
type: docs
url: /de/net/aspose.cells/hyperlink/area/
---
## Hyperlink.Area property

Ermittelt den Bereich des Hyperlinks.

```csharp
public CellArea Area { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Main Menu");
            worksheet.Cells["A3"].PutValue("Chapter 1");
            worksheet.Cells["A4"].PutValue("Chapter 2");
            
            // Hyperlinks hinzufügen
            int hyperlinkIndex1 = worksheet.Hyperlinks.Add("A3", 1, 1, "Sheet2!A1");
            int hyperlinkIndex2 = worksheet.Hyperlinks.Add("A4", 1, 1, "Sheet3!A1");

            // Hyperlinks zugreifen und die Verwendung der Area-Eigenschaft demonstrieren
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            string chapter2Address = "";
            foreach (Hyperlink link in hyperlinks)
            {
                // Überprüfen, ob sich ein Hyperlink in Zelle A4 befindet, mithilfe der Area-Eigenschaft
                if (link.Area.StartRow == 3 && link.Area.StartColumn == 0)
                {
                    chapter2Address = link.Address;
                    break;
                }
            }

            Console.WriteLine("Chapter 2 hyperlink address: " + chapter2Address);
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


