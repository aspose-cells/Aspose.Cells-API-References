---
title: "Range.ColumnWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Устанавливает или получает ширину столбца этого диапазона"
type: docs
url: /ru/net/aspose.cells/range/columnwidth/
---
## Range.ColumnWidth property

Устанавливает или получает ширину столбца этого диапазона.

```csharp
public double ColumnWidth { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к диапазону (столбцы B-D)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
            
            // Отобразите текущую ширину столбца
            Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);

            // Установите новую ширину столбца (в символьных единицах)
            range.ColumnWidth = 15.0;

            // Заполните ячейки, чтобы продемонстрировать эффект
            worksheet.Cells["B1"].PutValue("This is column B");
            worksheet.Cells["C1"].PutValue("This is column C");
            worksheet.Cells["D1"].PutValue("This is column D");

            // Автоматически подгонять строки, чтобы отобразить содержимое
            worksheet.AutoFitRows();

            // Сохраните книгу
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


