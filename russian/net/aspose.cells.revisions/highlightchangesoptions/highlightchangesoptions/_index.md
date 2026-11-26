---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор HighlightChangesOptions. Представляет параметры выделения ревизий или изменений в общих файлах Excel"
type: docs
url: /ru/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Представляет параметры выделения ревизий или изменений в совместных файлах Excel.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| highlightOnScreen | Boolean | Указывает, включено ли выделение изменений на экране. |
| listOnNewSheet | Boolean | Указывает, включено ли перечисление изменений на новом листе. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте некоторые образцы данных.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Создать HighlightChangesOptions с булевыми параметрами
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // Смоделировать отслеживание изменений (обычно у вас есть реальные ревизии)
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // Сохраните книгу
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### См. также

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


