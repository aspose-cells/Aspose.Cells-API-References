---
title: "Workbook.Theme"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает название темы"
type: docs
url: /ru/net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

Получает название темы.

```csharp
public string Theme { get; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyThemeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Продемонстрируйте получение темы по умолчанию
            Console.WriteLine("Default theme: " + workbook.Theme);
            
            // Измените цвет темы и проверьте
            workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
            Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
            Console.WriteLine("Modified Accent1 color: " + accent1);
            
            // Сохраните книгу, чтобы продемонстрировать сохранение темы
            workbook.Save("ThemeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


