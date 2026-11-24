---
title: "Klasse SmartTagSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Markup.SmartTagSetting‑Klasse. Stellt alle SmartTagCollection‑Objekte im Arbeitsblatt dar"
type: docs
url: /de/net/aspose.cells.markup/smarttagsetting/
---
## SmartTagSetting class

Stellt alle [`SmartTagCollection`](../smarttagcollection/)‑Objekte im Arbeitsblatt dar.

```csharp
public class SmartTagSetting : CollectionBase
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | Ruft ein [`SmartTagCollection`](../smarttagcollection/)‑Objekt über den Index ab. (3 Indexer) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | Füge ein Zellen‑SmartTag hinzu. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | Fügt einer Zelle ein [`SmartTagCollection`](../smarttagcollection/)‑Objekt hinzu. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingDemo
    {
        public static void SmartTagSettingExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einer bestimmten Zelle ein SmartTag hinzu
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // Greife auf die SmartTagCollection der Zelle zu
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // Füge der Sammlung ein SmartTag hinzu
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // Setze die Kapazität der SmartTag-Einstellung
            smartTagSetting.Capacity = 10;

            // Gib die Anzahl der SmartTags aus
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // Speichere die Arbeitsmappe
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


