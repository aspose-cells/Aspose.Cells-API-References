---
title: "Перечисление TxtValueQuoteType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.TxtValueQuoteType. Указывает тип использования кавычек для значений в файлах текстового формата"
type: docs
url: /ru/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

Указывает тип использования кавычек для значений в файлах текстового формата.

```csharp
public enum TxtValueQuoteType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Normal | `0` | Все значения, содержащие специальные символы, такие как кавычка или разделитель, будут заключены в кавычки. Такое же поведение, как у MS Excel при экспорте текстового файла. |
| Always | `1` | Все значения всегда будут заключены в кавычки. |
| Minimum | `2` | Кавычки ставятся только при необходимости. Например, если значение содержит кавычку, но кавычка не находится в начале значения, оно не будет заключено в кавычки. |
| Never | `3` | Все значения не будут заключены в кавычки. Экспортированный текстовый файл с этим типом может быть прочитан некорректно, поскольку необходимые кавычки отсутствуют. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtValueQuoteTypeDemo
    {
        public static void TxtValueQuoteTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells[0, 0].Value = "Name";
            worksheet.Cells[0, 1].Value = "Age";
            worksheet.Cells[1, 0].Value = "John Doe";
            worksheet.Cells[1, 1].Value = 30;
            worksheet.Cells[2, 0].Value = "Jane Smith";
            worksheet.Cells[2, 1].Value = 25;

            // Создайте TxtSaveOptions и задайте QuoteType
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.QuoteType = TxtValueQuoteType.Always;

            // Сохраните книгу как текстовый файл с указанным типом кавычек
            workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);

            Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


