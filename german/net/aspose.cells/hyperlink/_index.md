---
title: "Klasse Hyperlink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Hyperlink-Klasse. Kapselt das Objekt, das einen Hyperlink darstellt"
type: docs
url: /de/net/aspose.cells/hyperlink/
---
## Hyperlink class

Kapselt das Objekt, das einen Hyperlink darstellt.

```csharp
public class Hyperlink
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | Stellt die Adresse eines Hyperlinks dar. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | Ermittelt den Bereich des Hyperlinks. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | Ermittelt den Linktyp. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | Gibt den ScreenTip-Text für den angegebenen Hyperlink zurück oder legt ihn fest. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | Stellt den Text dar, der für den angegebenen Hyperlink angezeigt wird. Der Standardwert ist die Adresse des Hyperlinks. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | Löscht diesen Hyperlink |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkDemo
    {
        public static void HyperlinkExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            
            // Hinzufügen eines neuen Arbeitsblatts zum Workbook-Objekt
            workbook.Worksheets.Add();
            
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hinzufügen eines Hyperlinks zu einer URL in Zelle "A1"
            int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
            
            // Abrufen eines Hyperlinks nach Index
            Hyperlink hyperlink = worksheet.Hyperlinks[index];
            
            // Festlegen des Anzeigetextes dieses Hyperlinks
            hyperlink.TextToDisplay = "Aspose";
            
            // Festlegen des ScreenTip-Texts für den Hyperlink
            hyperlink.ScreenTip = "Visit Aspose Website";
            
            // Die Excel-Datei speichern
            workbook.Save("HyperlinkExample.xlsx");
            workbook.Save("HyperlinkExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


