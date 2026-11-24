---
title: "HyperlinkCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HyperlinkCollection-Eigenschaft. Gibt das Hyperlink-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

Gibt das [`Hyperlink`](../../hyperlink/) Element am angegebenen Index zurück.

```csharp
public Hyperlink this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einen Hyperlink zu Zelle A1 hinzu
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
            
            // Greifen Sie über die Item‑Eigenschaft auf den ersten Hyperlink zu und setzen Sie den Anzeigetext
            worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
            
            // Legen Sie den Hyperlink‑Stil fest (blauer unterstrichener Text)
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.Underline = FontUnderlineType.Single;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


