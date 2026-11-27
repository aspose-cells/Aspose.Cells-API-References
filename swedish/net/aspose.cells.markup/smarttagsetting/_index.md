---
title: "Klass SmartTagSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markup.SmartTagSetting-klass. Representerar alla SmartTagCollection-objekt i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.markup/smarttagsetting/
---
## SmartTagSetting class

Representerar alla [`SmartTagCollection`](../smarttagcollection/) objekt i kalkylbladet.

```csharp
public class SmartTagSetting : CollectionBase
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | Hämtar ett [`SmartTagCollection`](../smarttagcollection/) objekt efter index. (3 indexerare) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | Lägg till en smart tagg i cellen. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | Lägger till ett [`SmartTagCollection`](../smarttagcollection/) objekt i en cell. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en smart tagg i en specifik cell
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // Åtkomst till SmartTagCollection för cellen
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // Lägg till en smart tagg i samlingen
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // Ställ in kapaciteten för smart tagg-inställningen
            smartTagSetting.Capacity = 10;

            // Skriv ut antalet smarta taggar
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // Spara arbetsboken
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


