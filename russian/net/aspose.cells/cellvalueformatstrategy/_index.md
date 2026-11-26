---
title: "Перечисление CellValueFormatStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.CellValueFormatStrategy. Указывает, как применять стиль к значению ячейки"
type: docs
url: /ru/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

Указывает, как применять стиль к значению ячейки.

```csharp
public enum CellValueFormatStrategy
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Не отформатировано. |
| CellStyle | `1` | Отформатировано только оригинальным стилем ячейки. |
| DisplayStyle | `2` | Отформатировано отображаемым стилем ячейки. |
| DisplayString | `3` | Получает отображаемую строку, показываемую в MS Excel. Основное отличие от DisplayStyle заключается в том, что эта опция также учитывает влияние ширины столбца. Если ширина столбца слишком мала, чтобы полностью показать отформатированную строку, может отображаться "#", как в MS Excel. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueFormatStrategyDemo
    {
        public static void CellValueFormatStrategyExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Number");
            worksheet.Cells["B2"].PutValue(12345.6789);
            worksheet.Cells["C1"].PutValue("Text");
            worksheet.Cells["C2"].PutValue("Hello World");

            // Примените различные CellValueFormatStrategy, чтобы продемонстрировать их эффекты
            // None: Не отформатировано
            string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($"None: {valueNone}");

            // CellStyle: Отформатировано только оригинальным стилем ячейки
            string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($"CellStyle: {valueCellStyle}");

            // DisplayStyle: Отформатировано отображаемым стилем ячейки
            string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");

            // DisplayString: Получает отображаемую строку, показываемую в MS Excel
            string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($"DisplayString: {valueDisplayString}");

            // Сохранить книгу в файл
            workbook.Save("CellValueFormatStrategyExample.xlsx");
            workbook.Save("CellValueFormatStrategyExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


