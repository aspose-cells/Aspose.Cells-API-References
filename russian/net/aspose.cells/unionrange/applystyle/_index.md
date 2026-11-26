---
title: "UnionRange.ApplyStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Применяет форматы ко всему диапазону"
type: docs
url: /ru/net/aspose.cells/unionrange/applystyle/
---
## UnionRange.ApplyStyle method

Применяет форматы ко всему диапазону.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Объект стиля, который будет применён. |
| флаг | StyleFlag | Флаги, указывающие применённые свойства форматирования. |

### Примечания

Каждая ячейка в этом диапазоне будет содержать объект [`Style`](../../style/). Поэтому этот метод потребляет много памяти. Пожалуйста, используйте его осторожно.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте объединённый диапазон, охватывающий ячейки A1 до B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "More Data";

            try
            {
                // Создайте стиль с определённым форматированием
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.Font.Color = Color.Red;
                style.ForegroundColor = Color.LightBlue;
                style.Pattern = BackgroundType.Solid;
                style.HorizontalAlignment = TextAlignmentType.Center;

                // Создайте StyleFlag, чтобы указать, какие свойства применять
                StyleFlag flag = new StyleFlag();
                flag.FontBold = true;
                flag.FontColor = true;
                flag.CellShading = true;
                flag.HorizontalAlignment = true;

                // Вызовите ApplyStyle с параметрами стиля и флага
                unionRange.ApplyStyle(style, flag);

                Console.WriteLine("ApplyStyle method called successfully");
                Console.WriteLine($"Applied style to range: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ApplyStyle: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("UnionRangeMethodApplyStyleWithStyleStyleFlagDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


