---
title: "Перечисление PaneStateType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.PaneStateType. Представляет состояние области листов."
type: docs
url: /ru/net/aspose.cells/panestatetype/
---
## PaneStateType enumeration

Представляет состояние области листа.

```csharp
public enum PaneStateType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Frozen | `0` | Области заморожены, но до заморозки не были. |
| FrozenSplit | `1` | Области заморожены и были разделены до заморозки. |
| Split | `2` | Области разделены, но не заморожены. |
| Normal | `3` | Области не заморожены и не разделены. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PaneStateTypeDemo
    {
        public static void PaneStateTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить некоторые примерные данные в листе
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Заморозить области в ячейке B2
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Проверить состояние области
            PaneStateType paneState = worksheet.PaneState;

            // Вывести состояние области
            Console.WriteLine("Current Pane State: " + paneState);

            // Сохраните книгу
            workbook.Save("PaneStateTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


