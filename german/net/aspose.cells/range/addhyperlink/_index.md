---
title: "Range.AddHyperlink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu"
type: docs
url: /de/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| address | String | Adresse des Hyperlinks. |
| textToDisplay | String | Der Text, der für den angegebenen Hyperlink angezeigt werden soll. |
| screenTip | String | Der ScreenTip-Text für den angegebenen Hyperlink. |

### Rückgabewert

[`Hyperlink`](../../hyperlink/) object.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // Füge einen Hyperlink mit Adresse, Anzeigetext und Bildschirmtipp hinzu
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // Speichere die Arbeitsmappe
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


