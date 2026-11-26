---
title: "Cells.GetViewColumnWidthPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получить ширину в разных типах представления"
type: docs
url: /ru/net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

Получает ширину в разных типах представления.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

ширина столбца в пикселях

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите тип представления в PageLayoutView
            worksheet.ViewType = ViewType.PageLayoutView;
            
            // Установить ширину столбца в символах (будет преобразовано в пиксели)
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Получить ширину столбца в пикселях
            int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
            
            // Вывести результат.
            Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
            
            // Сохраните книгу
            workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


