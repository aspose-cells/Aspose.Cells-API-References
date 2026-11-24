---
title: "Enum UpdateLinksType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.UpdateLinksType enum. Gibt an, wie Links zu anderen Arbeitsmappen beim Öffnen der Arbeitsmappe aktualisiert werden"
type: docs
url: /de/net/aspose.cells/updatelinkstype/
---
## UpdateLinksType enumeration

Stellt dar, wie Links zu anderen Arbeitsmappen beim Öffnen der Arbeitsmappe aktualisiert werden.

```csharp
public enum UpdateLinksType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| UserSet | `0` | Benutzer zur Aktualisierung auffordern. |
| Never | `1` | Nicht aktualisieren und den Benutzer nicht auffordern. |
| Always | `2` | Immer aktualisieren. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UpdateLinksTypeDemo
    {
        public static void UpdateLinksTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf die Arbeitsmappeneinstellungen zu
            WorkbookSettings settings = workbook.Settings;

            // Setzen Sie den UpdateLinksType auf Immer aktualisieren
            settings.UpdateLinksType = UpdateLinksType.Always;

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("External Link Example");
            worksheet.Cells["A2"].PutValue("Data");

            // Speichere die Arbeitsmappe
            workbook.Save("UpdateLinksTypeExample.xlsx");

            // Geben Sie die aktuelle Einstellung des UpdateLinksType aus
            Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


