---
title: "Перечисление TargetModeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.TargetModeType. Представляет тип целевого режима"
type: docs
url: /ru/net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

Представляет тип целевого режима.

```csharp
public enum TargetModeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| External | `0` | Внешняя ссылка |
| FilePath | `1` | Локальные и полные пути к файлам или папкам. |
| Email | `2` | Электронная почта. |
| CellReference | `3` | Ссылка на ячейку или именованный диапазон. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTargetModeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить внешнюю гиперссылку
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Получить гиперссылку и проверить её TargetModeType
            Hyperlink link = worksheet.Hyperlinks[0];
            Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
            
            // Удалить гиперссылку
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


