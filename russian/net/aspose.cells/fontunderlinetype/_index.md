---
title: "Перечисление FontUnderlineType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.FontUnderlineType. Перечисляет типы подчеркивания шрифта"
type: docs
url: /ru/net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

Перечисляет типы подчеркивания шрифта.

```csharp
public enum FontUnderlineType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Обозначает отсутствие подчеркивания. |
| Single | `1` | Обозначает одинарное подчеркивание. |
| Double | `2` | Обозначает двойное подчеркивание. |
| Accounting | `3` | Обозначает одинарное бухгалтерское подчеркивание. |
| DoubleAccounting | `4` | Обозначает двойное бухгалтерское подчеркивание. |
| Dash | `5` | Обозначает пунктирное подчеркивание |
| DashDotDotHeavy | `6` | Обозначает толстое подчеркивание тире-точка-точка |
| DashDotHeavy | `7` | Обозначает толстое подчеркивание тире-точка |
| DashedHeavy | `8` | Обозначает толстое пунктирное подчеркивание |
| DashLong | `9` | Обозначает длинное пунктирное подчеркивание |
| DashLongHeavy | `10` | Обозначает толстое длинное пунктирное подчеркивание |
| DotDash | `11` | Обозначает подчеркивание тире-точка |
| DotDotDash | `12` | Обозначает подчеркивание тире-точка-точка |
| Dotted | `13` | Обозначает точечное подчеркивание |
| DottedHeavy | `14` | Обозначает толстое точечное подчеркивание |
| Heavy | `15` | Обозначает толстое подчеркивание |
| Wave | `16` | Представляет волнистое подчеркивание |
| WavyDouble | `17` | Представляет двойное волнистое подчеркивание |
| WavyHeavy | `18` | Представляет тяжелое волнистое подчеркивание |
| Words | `19` | Представляет подчеркивание символов, не являющихся пробелами. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить ссылку на первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к ячейке "A1" листа
            Cell cell = worksheet.Cells["A1"];
            
            // Добавление некоторого значения в ячейку "A1"
            cell.PutValue("Hello Aspose!");

            // Получить стиль ячейки
            Style style = cell.GetStyle();
            
            // Установить тип подчеркивания шрифта в одинарное подчеркивание
            style.Font.Underline = FontUnderlineType.Single;
            
            // Применить стиль к ячейке
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


