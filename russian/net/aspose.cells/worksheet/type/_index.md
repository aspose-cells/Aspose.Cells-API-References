---
title: "Worksheet.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Представляет тип листа"
type: docs
url: /ru/net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Представляет тип листа.

```csharp
public SheetType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите некоторые базовые свойства
            worksheet.Name = "DemoSheet";
            worksheet.IsVisible = true;
            
            // Продемонстрировать использование свойства Type
            Console.WriteLine("Worksheet Type: " + worksheet.Type);
            
            // Добавьте лист диаграммы, чтобы продемонстрировать различные типы листов
            workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[1];
            
            // Сравните типы листов
            Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
            Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
            
            // Сохраните книгу
            workbook.Save("WorksheetTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


