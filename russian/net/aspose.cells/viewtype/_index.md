---
title: "Перечисление ViewType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ViewType. Представляет тип представления листа"
type: docs
url: /ru/net/aspose.cells/viewtype/
---
## ViewType enumeration

Представляет тип представления листа.

```csharp
public enum ViewType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ViewTypeDemo
    {
        public static void ViewTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите тип представления листа в PageBreakPreview
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // Сохраните книгу
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


