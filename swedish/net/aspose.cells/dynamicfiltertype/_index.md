---
title: "Enum DynamicFilterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DynamicFilterType enum. Dynamisk filtertyp"
type: docs
url: /sv/net/aspose.cells/dynamicfiltertype/
---
## DynamicFilterType enumeration

Dynamisk filtertyp.

```csharp
public enum DynamicFilterType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| AboveAverage | `0` | Visar värden som är över genomsnittet. |
| BelowAverage | `1` | Visar värden som är under genomsnittet. |
| LastMonth | `2` | Visar förra månadens datum. |
| LastQuarter | `3` | Visar förra kvartalets datum. |
| LastWeek | `4` | Visar förra veckans datum. |
| LastYear | `5` | Visar förra årets datum. |
| January | `6` | Visar datum som är i januari, oavsett år. |
| October | `7` | Visar datum som är i oktober, oavsett år. |
| November | `8` | Visar datum som är i november, oavsett år. |
| December | `9` | Visar datum som är i december, oavsett år. |
| February | `10` | Visar datum som är i februari, oavsett år. |
| March | `11` | Visar datum som är i mars, oavsett år. |
| April | `12` | Visar datum som är i april, oavsett år. |
| May | `13` | Visar datum som är i maj, oavsett år. |
| June | `14` | Visar datum som är i juni, oavsett år. |
| July | `15` | Visar datumen som är i juli, oavsett år. |
| August | `16` | Visar datumen som är i augusti, oavsett år. |
| September | `17` | Visar datumen som är i september, oavsett år. |
| NextMonth | `18` | Visar nästa månads datum. |
| NextQuarter | `19` | Visar nästa kvartals datum. |
| NextWeek | `20` | Visar nästa veckas datum. |
| NextYear | `21` | Visar nästa års datum. |
| None | `22` | Ingen. |
| Quarter1 | `23` | Visar datumen som är i första kvartalet, oavsett år. |
| Quarter2 | `24` | Visar datumen som är i andra kvartalet, oavsett år. |
| Quarter3 | `25` | Visar datumen som är i tredje kvartalet, oavsett år. |
| Quarter4 | `26` | Visar datumen som är i fjärde kvartalet, oavsett år. |
| ThisMonth | `27` | Visar den här månadens datum. |
| ThisQuarter | `28` | Visar detta kvartals datum. |
| ThisWeek | `29` | Visar denna veckas datum. |
| ThisYear | `30` | Visar detta års datum. |
| Today | `31` | Visar dagens datum. |
| Tomorrow | `32` | Visar morgondagens datum. |
| YearToDate | `33` | Visar datumen mellan början av året och idag, inklusive. |
| Yesterday | `34` | Visar gårdagens datum. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterTypeDemo
    {
        public static void DynamicFilterTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // Applicera autofilter på kalkylbladet
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Applicera ett dynamiskt filter för att endast visa datum i mars
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Spara arbetsboken
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // Skriv ut resultaten
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


