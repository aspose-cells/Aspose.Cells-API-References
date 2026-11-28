---
title: "Enum CountryCode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CountryCode enum. Excel ülke tanımlayıcılarını temsil eder"
type: docs
url: /tr/net/aspose.cells/countrycode/
---
## CountryCode enumeration

Excel ülke tanımlayıcılarını temsil eder.

```csharp
public enum CountryCode
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` |  |
| USA | `1` | Amerika Birleşik Devletleri |
| Canada | `2` | Kanada |
| LatinAmeric | `3` | Brezilya hariç Latin Amerika |
| Russia | `7` | Rusya |
| Egypt | `20` | Mısır |
| Greece | `30` | Yunanistan |
| Netherlands | `31` | Hollanda |
| Belgium | `32` | Belçika |
| France | `33` | Fransa |
| Spain | `34` | İspanya |
| Hungary | `36` | Macaristan |
| Italy | `39` | İtalya |
| Switzerland | `41` | İsviçre |
| Austria | `43` | Avusturya |
| UnitedKingdom | `44` | Birleşik Krallık |
| Denmark | `45` | Danimarka |
| Sweden | `46` | İsveç |
| Norway | `47` | Norveç |
| Poland | `48` | Polonya |
| Germany | `49` | Almanya |
| Mexico | `52` | Meksika |
| Brazil | `55` | Brezilya |
| Australia | `61` | Avustralya |
| NewZealand | `64` | Yeni Zelanda |
| Thailand | `66` | Tayland |
| Japan | `81` | Japonya |
| SouthKorea | `82` | Güney Kore |
| VietNam | `84` | Vietnam |
| China | `86` | Çin Halk Cumhuriyeti |
| Turkey | `90` | Türkiye |
| India | `91` | Hindistan |
| Algeria | `213` | Cezayir |
| Morocco | `216` | Fas |
| Libya | `218` | Libya |
| Portugal | `351` | Portekiz |
| Iceland | `354` | İzlanda |
| Finland | `358` | Finlandiya |
| Czech | `420` | Çek Cumhuriyeti |
| Taiwan | `886` | Tayvan |
| Lebanon | `961` | Lübnan |
| Jordan | `962` | Ürdün |
| Syria | `963` | Suriye |
| Iraq | `964` | Irak |
| Kuwait | `965` | Kuveyt |
| Saudi | `966` | Suudi Arabistan |
| UnitedArabEmirates | `971` | Birleşik Arap Emirlikleri |
| Israel | `972` | İsrail |
| Qatar | `974` | Katar |
| Iran | `981` | İran |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CountryCodeDemo
    {
        public static void CountryCodeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma kitabı için ülke kodunu ayarla
            workbook.Settings.LanguageCode = CountryCode.USA;
            workbook.Settings.Region = CountryCode.USA;

            // Çalışma sayfasına bazı veriler ekle
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

            // Çalışma kitabını kaydedin
            workbook.Save("CountryCodeExample.xlsx");
            workbook.Save("CountryCodeExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


