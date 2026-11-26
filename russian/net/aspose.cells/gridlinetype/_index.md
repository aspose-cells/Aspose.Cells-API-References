---
title: "Перечисление GridlineType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.GridlineType. Перечисляет типы линий сетки"
type: docs
url: /ru/net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

Перечисляет тип линий сетки.

```csharp
public enum GridlineType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Dotted | `0` | Представляет пунктирную линию. |
| Hair | `1` | Представляет тонкую линию. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGridlineTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте параметры сохранения и задайте тип линий сетки
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.GridlineType = GridlineType.Dotted;
            
            // Добавьте некоторые примерные данные, чтобы увидеть линии сетки
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            // Сохраните книгу с параметрами сохранения
            workbook.Save("GridlineTypeDemo.docx", saveOptions);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


