---
title: "Перечисление TableStyleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Tables.TableStyleType. Представляет встроенный тип стиля таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestyletype/
---
## TableStyleType enumeration

Представляет тип встроенного стиля таблицы.

```csharp
public enum TableStyleType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без стиля. |
| TableStyleLight1 | `1` | Стиль таблицы Light 1 |
| TableStyleLight2 | `2` |  |
| TableStyleLight3 | `3` |  |
| TableStyleLight4 | `4` |  |
| TableStyleLight5 | `5` |  |
| TableStyleLight6 | `6` |  |
| TableStyleLight7 | `7` |  |
| TableStyleLight8 | `8` |  |
| TableStyleLight9 | `9` |  |
| TableStyleLight10 | `10` |  |
| TableStyleLight11 | `11` |  |
| TableStyleLight12 | `12` |  |
| TableStyleLight13 | `13` |  |
| TableStyleLight14 | `14` |  |
| TableStyleLight15 | `15` |  |
| TableStyleLight16 | `16` |  |
| TableStyleLight17 | `17` |  |
| TableStyleLight18 | `18` |  |
| TableStyleLight19 | `19` |  |
| TableStyleLight20 | `20` |  |
| TableStyleLight21 | `21` |  |
| TableStyleMedium1 | `22` |  |
| TableStyleMedium2 | `23` |  |
| TableStyleMedium3 | `24` |  |
| TableStyleMedium4 | `25` |  |
| TableStyleMedium5 | `26` |  |
| TableStyleMedium6 | `27` |  |
| TableStyleMedium7 | `28` |  |
| TableStyleMedium8 | `29` |  |
| TableStyleMedium9 | `30` |  |
| TableStyleMedium10 | `31` |  |
| TableStyleMedium11 | `32` |  |
| TableStyleMedium12 | `33` |  |
| TableStyleMedium13 | `34` |  |
| TableStyleMedium14 | `35` |  |
| TableStyleMedium15 | `36` |  |
| TableStyleMedium16 | `37` |  |
| TableStyleMedium17 | `38` |  |
| TableStyleMedium18 | `39` |  |
| TableStyleMedium19 | `40` |  |
| TableStyleMedium20 | `41` |  |
| TableStyleMedium21 | `42` |  |
| TableStyleMedium22 | `43` |  |
| TableStyleMedium23 | `44` |  |
| TableStyleMedium24 | `45` |  |
| TableStyleMedium25 | `46` |  |
| TableStyleMedium26 | `47` |  |
| TableStyleMedium27 | `48` |  |
| TableStyleMedium28 | `49` |  |
| TableStyleDark1 | `50` |  |
| TableStyleDark2 | `51` |  |
| TableStyleDark3 | `52` |  |
| TableStyleDark4 | `53` |  |
| TableStyleDark5 | `54` |  |
| TableStyleDark6 | `55` |  |
| TableStyleDark7 | `56` |  |
| TableStyleDark8 | `57` |  |
| TableStyleDark9 | `58` |  |
| TableStyleDark10 | `59` |  |
| TableStyleDark11 | `60` |  |
| Custom | `61` |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleTypeDemo
    {
        public static void TableStyleTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Создайте ListObject (таблицу) на листе
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Установите тип стиля таблицы
            listObject.TableStyleType = TableStyleType.TableStyleMedium2;

            // Установить дополнительные свойства для таблицы
            listObject.ShowHeaderRow = true;
            listObject.ShowTotals = true;
            listObject.ShowTableStyleFirstColumn = true;
            listObject.ShowTableStyleLastColumn = true;
            listObject.ShowTableStyleRowStripes = true;
            listObject.ShowTableStyleColumnStripes = true;

            // Сохраните книгу
            workbook.Save("TableStyleTypeExample.xlsx");

            // Вывести тип стиля таблицы
            Console.WriteLine("Table Style Type: " + listObject.TableStyleType);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


