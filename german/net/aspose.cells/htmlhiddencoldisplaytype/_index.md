---
title: "Enum HtmlHiddenColDisplayType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlHiddenColDisplayType Aufzählung. Stellt zwei Arten dar, versteckte Spalten in HTML anzuzeigen"
type: docs
url: /de/net/aspose.cells/htmlhiddencoldisplaytype/
---
## HtmlHiddenColDisplayType enumeration

Stellt zwei Arten dar, versteckte Spalten in HTML anzuzeigen.

```csharp
public enum HtmlHiddenColDisplayType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Hidden | `0` | Versteckt die versteckten Spalten auf der HTML‑Seite. |
| Remove | `1` | Entfernt die versteckten Spalten auf der HTML‑Seite. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenColDisplayTypeDemo
    {
        public static void HtmlHiddenColDisplayTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Zweite Spalte ausblenden
            worksheet.Cells.HideColumn(1);

            // Erstelle HtmlSaveOptions und setze den HiddenColDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;

            // Speichere das Arbeitsbuch im HTML‑Format
            workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


