---
title: "Enum CountryCode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CountryCode‑enum. Representerar Excel-landskoder"
type: docs
url: /sv/net/aspose.cells/countrycode/
---
## CountryCode enumeration

Representerar Excel-landidentifierare.

```csharp
public enum CountryCode
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` |  |
| USA | `1` | USA |
| Canada | `2` | Kanada |
| LatinAmeric | `3` | Latinamerika, förutom Brasilien |
| Russia | `7` | Ryssland |
| Egypt | `20` | Egypten |
| Greece | `30` | Grekland |
| Netherlands | `31` | Nederländerna |
| Belgium | `32` | Belgien |
| France | `33` | Frankrike |
| Spain | `34` | Spanien |
| Hungary | `36` | Ungern |
| Italy | `39` | Italien |
| Switzerland | `41` | Schweiz |
| Austria | `43` | Österrike |
| UnitedKingdom | `44` | Storbritannien |
| Denmark | `45` | Danmark |
| Sweden | `46` | Sverige |
| Norway | `47` | Norge |
| Poland | `48` | Polen |
| Germany | `49` | Tyskland |
| Mexico | `52` | Mexiko |
| Brazil | `55` | Brasilien |
| Australia | `61` | Australien |
| NewZealand | `64` | Nya Zeeland |
| Thailand | `66` | Thailand |
| Japan | `81` | Japan |
| SouthKorea | `82` | Sydkorea |
| VietNam | `84` | Vietnam |
| China | `86` | Folkrepubliken Kina |
| Turkey | `90` | Turkiet |
| India | `91` | Indien |
| Algeria | `213` | Algeriet |
| Morocco | `216` | Marocko |
| Libya | `218` | Libyen |
| Portugal | `351` | Portugal |
| Iceland | `354` | Island |
| Finland | `358` | Finland |
| Czech | `420` | Tjeckien |
| Taiwan | `886` | Taiwan |
| Lebanon | `961` | Libanon |
| Jordan | `962` | Jordanien |
| Syria | `963` | Syrien |
| Iraq | `964` | Irak |
| Kuwait | `965` | Kuwait |
| Saudi | `966` | Saudiarabien |
| UnitedArabEmirates | `971` | Förenade Arabemiraten |
| Israel | `972` | Israel |
| Qatar | `974` | Qatar |
| Iran | `981` | Iran |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CountryCodeDemo
    {
        public static void CountryCodeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange landskoden för arbetsboken
            workbook.Settings.LanguageCode = CountryCode.USA;
            workbook.Settings.Region = CountryCode.USA;

            // Lägg till lite data i kalkylbladet
            worksheet.Cells[0, 0].PutValue("Country");
            worksheet.Cells[0, 1].PutValue("Code");

            worksheet.Cells[1, 0].PutValue("United States");
            worksheet.Cells[1, 1].PutValue((int)CountryCode.USA);

            worksheet.Cells[2, 0].PutValue("Canada");
            worksheet.Cells[2, 1].PutValue((int)CountryCode.Canada);

            worksheet.Cells[3, 0].PutValue("France");
            worksheet.Cells[3, 1].PutValue((int)CountryCode.France);

            worksheet.Cells[4, 0].PutValue("Germany");
            worksheet.Cells[4, 1].PutValue((int)CountryCode.Germany);

            // Spara arbetsboken
            workbook.Save("CountryCodeExample.xlsx");
            workbook.Save("CountryCodeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


