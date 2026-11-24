---
title: "Enum CountryCode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CountryCode enum. Stellt Excel-Länderkürzel dar."
type: docs
url: /de/net/aspose.cells/countrycode/
---
## CountryCode enumeration

Stellt Excel‑Länderkürzel dar.

```csharp
public enum CountryCode
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` |  |
| USA | `1` | Vereinigte Staaten |
| Canada | `2` | Kanada |
| LatinAmeric | `3` | Lateinamerika, außer Brasilien |
| Russia | `7` | Russland |
| Egypt | `20` | Ägypten |
| Greece | `30` | Griechenland |
| Netherlands | `31` | Niederlande |
| Belgium | `32` | Belgien |
| France | `33` | Frankreich |
| Spain | `34` | Spanien |
| Hungary | `36` | Ungarn |
| Italy | `39` | Italien |
| Switzerland | `41` | Schweiz |
| Austria | `43` | Österreich |
| UnitedKingdom | `44` | Vereinigtes Königreich |
| Denmark | `45` | Dänemark |
| Sweden | `46` | Schweden |
| Norway | `47` | Norwegen |
| Poland | `48` | Polen |
| Germany | `49` | Deutschland |
| Mexico | `52` | Mexiko |
| Brazil | `55` | Brasilien |
| Australia | `61` | Australien |
| NewZealand | `64` | Neuseeland |
| Thailand | `66` | Thailand |
| Japan | `81` | Japan |
| SouthKorea | `82` | Südkorea |
| VietNam | `84` | Vietnam |
| China | `86` | Volksrepublik China |
| Turkey | `90` | Türkei |
| India | `91` | Indien |
| Algeria | `213` | Algerien |
| Morocco | `216` | Marokko |
| Libya | `218` | Libyen |
| Portugal | `351` | Portugal |
| Iceland | `354` | Island |
| Finland | `358` | Finnland |
| Czech | `420` | Tschechien |
| Taiwan | `886` | Taiwan |
| Lebanon | `961` | Libanon |
| Jordan | `962` | Jordanien |
| Syria | `963` | Syrien |
| Iraq | `964` | Irak |
| Kuwait | `965` | Kuwait |
| Saudi | `966` | Saudi-Arabien |
| UnitedArabEmirates | `971` | Vereinigte Arabische Emirate |
| Israel | `972` | Israel |
| Qatar | `974` | Katar |
| Iran | `981` | Iran |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CountryCodeDemo
    {
        public static void CountryCodeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Legen Sie den Ländercode für die Arbeitsmappe fest
            workbook.Settings.LanguageCode = CountryCode.USA;
            workbook.Settings.Region = CountryCode.USA;

            // Füge dem Arbeitsblatt einige Daten hinzu
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

            // Speichere die Arbeitsmappe
            workbook.Save("CountryCodeExample.xlsx");
            workbook.Save("CountryCodeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


