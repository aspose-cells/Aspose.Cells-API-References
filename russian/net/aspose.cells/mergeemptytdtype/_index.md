---
title: "Перечисление MergeEmptyTdType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.MergeEmptyTdType. Представляет тип слияния для пустого элемента TD при экспорте файла в HTML"
type: docs
url: /ru/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

Представляет тип объединения для пустого элемента TD при экспорте файла в HTML.

```csharp
public enum MergeEmptyTdType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Отображать как MS Excel. |
| None | `1` | Пустые элементы TD не будут объединяться при экспорте файла в html. Это приведёт к значительно большему html‑файлу. |
| MergeForcely | `2` | Принудительное объединение пустых элементов TD при экспорте файла в html. Размер html‑файла будет значительно уменьшен после установки значения в true. Если вы хотите импортировать html‑файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html, пожалуйста, оставьте значение по умолчанию. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // Создайте HtmlSaveOptions и установите свойство MergeEmptyTdType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // Сохраните книгу в формате HTML
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


