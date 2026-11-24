---
title: "HyperlinkCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HyperlinkCollection-Methode. Entfernt den Hyperlink am angegebenen Index in dieser Sammlung"
type: docs
url: /de/net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Entfernt den Hyperlink am angegebenen Index in dieser Sammlung.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der nullbasierte Index des Elements. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge einen Hyperlink zu Zelle A1 hinzu
            sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Überprüfen, ob der Hyperlink vor dem Entfernen existiert
            Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
            
            // Entferne den Hyperlink bei Index 0
            sheet.Hyperlinks.RemoveAt(0);
            
            // Überprüfen, ob der Hyperlink entfernt wurde
            Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
        }
    }
}
```

### Siehe auch

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


