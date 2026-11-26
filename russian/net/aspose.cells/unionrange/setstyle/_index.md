---
title: "UnionRange.SetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Устанавливает стиль диапазона"
type: docs
url: /ru/net/aspose.cells/unionrange/setstyle/
---
## UnionRange.SetStyle method

Устанавливает стиль диапазона.

```csharp
public void SetStyle(Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Объект Style. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните диапазон A1:B2 образцами данных
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue("Total");
            worksheet.Cells["B2"].PutValue(456);

            // Создайте UnionRange, охватывающий ячейки A1:B2
            UnionRange unionRange = worksheet.Cells
                .CreateRange("A1:B2")
                .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Создайте экземпляр Style и задайте некоторое форматирование
                Style style = new Style();
                style.BackgroundColor = Color.LightYellow;
                style.ForegroundColor = Color.DarkBlue;
                style.HorizontalAlignment = TextAlignmentType.Center;
                style.VerticalAlignment = TextAlignmentType.Center;
                style.IsTextWrapped = true;

                // Примените стиль к объединённому диапазону
                unionRange.SetStyle(style);

                Console.WriteLine("SetStyle executed successfully on the UnionRange.");

                // Сохраните книгу, чтобы визуализировать результат
                workbook.Save("UnionRangeSetStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetStyle: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


