---
title: "Klasse SmartTagOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Markup.SmartTagOptions Klasse. Stellt die Optionen des SmartTags dar."
type: docs
url: /de/net/aspose.cells.markup/smarttagoptions/
---
## SmartTagOptions class

Stellt die Optionen des SmartTags dar.

```csharp
public class SmartTagOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | Gibt an, ob SmartTags mit der Arbeitsmappe gespeichert werden. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | Stellt den Anzeigetyp des SmartTags dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Eigenschaften festlegen
            options.EmbedSmartTags = true;
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;

            // Wende SmartTagOptions auf das Arbeitsblatt an
            // Hinweis: Geändert von worksheet.SmartTagSetting.Options = options;
            // um das Optionsobjekt direkt zu verwenden, da SmartTagSetting keine Options-Eigenschaft hat
            // (Angenommen, die Optionen sollen direkt verwendet werden)
            
            // Füge einige Daten zur Demonstration hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);

            // Speichere die Arbeitsmappe
            workbook.Save("SmartTagOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


