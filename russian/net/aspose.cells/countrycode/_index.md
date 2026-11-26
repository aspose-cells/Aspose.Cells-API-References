---
title: "Перечисление CountryCode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.CountryCode. Представляет идентификаторы стран в Excel"
type: docs
url: /ru/net/aspose.cells/countrycode/
---
## CountryCode enumeration

Представляет идентификаторы стран Excel.

```csharp
public enum CountryCode
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` |  |
| USA | `1` | Соединённые Штаты |
| Canada | `2` | Канада |
| LatinAmeric | `3` | Латинская Америка, кроме Бразилии |
| Russia | `7` | Россия |
| Egypt | `20` | Египет |
| Greece | `30` | Греция |
| Netherlands | `31` | Нидерланды |
| Belgium | `32` | Бельгия |
| France | `33` | Франция |
| Spain | `34` | Испания |
| Hungary | `36` | Венгрия |
| Italy | `39` | Италия |
| Switzerland | `41` | Швейцария |
| Austria | `43` | Австрия |
| UnitedKingdom | `44` | Великобритания |
| Denmark | `45` | Дания |
| Sweden | `46` | Швеция |
| Norway | `47` | Норвегия |
| Poland | `48` | Польша |
| Germany | `49` | Германия |
| Mexico | `52` | Мексика |
| Brazil | `55` | Бразилия |
| Australia | `61` | Австралия |
| NewZealand | `64` | Новая Зеландия |
| Thailand | `66` | Таиланд |
| Japan | `81` | Япония |
| SouthKorea | `82` | Южная Корея |
| VietNam | `84` | Вьетнам |
| China | `86` | Китайская Народная Республика |
| Turkey | `90` | Турция |
| India | `91` | Индия |
| Algeria | `213` | Алжир |
| Morocco | `216` | Марокко |
| Libya | `218` | Ливия |
| Portugal | `351` | Португалия |
| Iceland | `354` | Исландия |
| Finland | `358` | Финляндия |
| Czech | `420` | Чешская Республика |
| Taiwan | `886` | Тайвань |
| Lebanon | `961` | Ливан |
| Jordan | `962` | Иордания |
| Syria | `963` | Сирия |
| Iraq | `964` | Ирак |
| Kuwait | `965` | Кувейт |
| Saudi | `966` | Саудовская Аравия |
| UnitedArabEmirates | `971` | Объединённые Арабские Эмираты |
| Israel | `972` | Израиль |
| Qatar | `974` | Катар |
| Iran | `981` | Иран |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CountryCodeDemo
    {
        public static void CountryCodeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите код страны для рабочей книги
            workbook.Settings.LanguageCode = CountryCode.USA;
            workbook.Settings.Region = CountryCode.USA;

            // Добавить некоторые данные в лист
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

            // Сохраните книгу
            workbook.Save("CountryCodeExample.xlsx");
            workbook.Save("CountryCodeExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


