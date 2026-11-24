---
title: "Enum DefaultEditLanguage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DefaultEditLanguage Enum. Stellt die standardmäßige Bearbeitungssprache dar"
type: docs
url: /de/net/aspose.cells/defaulteditlanguage/
---
## DefaultEditLanguage enumeration

Stellt die Standardsprache für die Bearbeitung dar.

```csharp
public enum DefaultEditLanguage
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Auto | `0` | Stellt die automatische Erkennung der Bearbeitungssprache anhand des Textes selbst dar. |
| English | `1` | Stellt die englische Sprache dar. |
| CJK | `2` | Stellt die chinesische, japanische und koreanische Sprache dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultEditLanguageDemo
    {
        public static void DefaultEditLanguageExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // AutoFitterOptions erstellen und DefaultEditLanguage festlegen
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Zeilen automatisch anpassen mit den angegebenen Optionen
            worksheet.AutoFitRows(autoFitterOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // Gib das festgelegte DefaultEditLanguage in der Konsole aus
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


