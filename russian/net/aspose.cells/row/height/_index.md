---
title: "Row.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Получает и задает высоту строки в единицах точек"
type: docs
url: /ru/net/aspose.cells/row/height/
---
## Row.Height property

Получает и задает высоту строки в единицах точек.

```csharp
public double Height { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите высоту строки для первой строки
            Row row = worksheet.Cells.Rows[0];
            row.Height = 30;
            
            // Добавьте некоторые данные в строку
            worksheet.Cells["A1"].PutValue("Row with custom height");
            
            // Проверьте и отобразите высоту строки
            Console.WriteLine("Row 1 Height: " + row.Height);
            
            // Сохраните книгу
            workbook.Save("RowHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


