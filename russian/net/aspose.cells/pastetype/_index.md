---
title: "Перечисление PasteType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.PasteType. Представляет тип специальной вставки"
type: docs
url: /ru/net/aspose.cells/pastetype/
---
## PasteType enumeration

Представляет тип специальной вставки.

```csharp
public enum PasteType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| All | `0` | Копирует все данные диапазона. |
| Default | `1` | Работает как поведение "All" в MS Excel. |
| AllExceptBorders | `2` | Копирует все данные диапазона без диапазона. |
| DefaultExceptBorders | `3` | Работает как поведение "All except borders" в MS Excel. |
| ColumnWidths | `4` | Копирует только ширины диапазона. |
| RowHeights | `5` | Копирует только высоты диапазона. |
| Comments | `6` | Копирует только комментарии в диапазоне. |
| Formats | `7` | Копирует только форматы в диапазоне. |
| Formulas | `8` | Копирует только формулы в диапазоне. |
| FormulasAndNumberFormats | `9` | Копирует только формулы и числовые форматы в диапазоне. |
| Validation | `10` | Копирует только проверки данных в диапазоне. |
| Values | `11` | Копирует только значения в диапазоне. |
| ValuesAndFormats | `12` | Копирует только значения и форматы в диапазоне. |
| ValuesAndNumberFormats | `13` | Копирует только значения и числовые форматы в диапазоне. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
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

            // Определите исходный диапазон
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // Определите диапазон назначения
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // Создайте PasteOptions и установите PasteType
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // Скопируйте исходный диапазон в диапазон назначения с указанными параметрами вставки
            destinationRange.Copy(sourceRange, pasteOptions);

            // Сохраните книгу
            workbook.Save("PasteTypeExample.xlsx");

            // Выведите результаты
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


