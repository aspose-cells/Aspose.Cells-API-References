---
title: "PageSetup.Orientation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет ориентацию печати страницы"
type: docs
url: /ru/net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Представляет ориентацию печати страницы.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrientationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить ориентацию страницы в альбомную
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            
            // Добавьте некоторые примерные данные, чтобы продемонстрировать эффект
            worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
            }
            
            // Сохраните книгу
            workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


