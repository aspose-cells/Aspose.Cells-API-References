---
title: "Перечисление AutoFitWrappedTextType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.AutoFitWrappedTextType. Представляет тип автоматической подгонки перенесённого текста"
type: docs
url: /ru/net/aspose.cells/autofitwrappedtexttype/
---
## AutoFitWrappedTextType enumeration

Представляет тип автоматической подгонки перенесённого текста.

```csharp
public enum AutoFitWrappedTextType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Работает как MS Excel. |
| Paragraph | `1` | Автоматически подгонять ширину по самому длинному абзацу. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitWrappedTextTypeDemo
    {
        public static void AutoFitWrappedTextTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
            worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");

            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            Style style2 = worksheet.Cells["A5"].GetStyle();
            style2.IsTextWrapped = true;
            worksheet.Cells["A5"].SetStyle(style);

            // Создайте диапазон A1:F3
            Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
            // Объедините ячейки
            range.Merge();

            // Создайте диапазон A4:F6
            Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
            // Объедините ячейки
            range2.Merge();

            // Создайте AutoFitterOptions и задайте AutoFitWrappedTextType
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            // Автоматически подгонять строки с указанными параметрами
            worksheet.AutoFitRows(options);

            // Сохраните книгу
            workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
            workbook.Save("AutoFitWrappedTextTypeExample.pdf");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


