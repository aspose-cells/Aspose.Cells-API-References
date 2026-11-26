---
title: "Range.CurrentRegion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает объект Range, представляющий текущий регион. Текущий регион — это диапазон, ограниченный любой комбинацией пустых строк и пустых столбцов"
type: docs
url: /ru/net/aspose.cells/range/currentregion/
---
## Range.CurrentRegion property

Возвращает объект Range, представляющий текущий регион. Текущий регион — это диапазон, ограниченный любой комбинацией пустых строк и пустых столбцов.

```csharp
public Range CurrentRegion { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyCurrentRegionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните данные некоторыми пустыми ячейками, чтобы создать регионы
            worksheet.Cells["A1"].PutValue("Region 1");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Оставьте строку 5 пустой, чтобы разделить регионы
            
            worksheet.Cells["A6"].PutValue("Region 2");
            worksheet.Cells["A7"].PutValue("Data 4");
            worksheet.Cells["B7"].PutValue("Data 5");
            worksheet.Cells["A8"].PutValue("Data 6");

            // Получите ячейку в первом регионе и преобразуйте её в Range
            Aspose.Cells.Range cellInRegion1 = worksheet.Cells.CreateRange("A2", "A2");
            Aspose.Cells.Range currentRegion1 = cellInRegion1.CurrentRegion;
            
            Console.WriteLine("CurrentRegion for A2: " + currentRegion1.Address);
            Console.WriteLine("Row count in region: " + currentRegion1.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion1.ColumnCount);

            // Получите ячейку во втором регионе и преобразуйте её в Range
            Aspose.Cells.Range cellInRegion2 = worksheet.Cells.CreateRange("B7", "B7");
            Aspose.Cells.Range currentRegion2 = cellInRegion2.CurrentRegion;
            
            Console.WriteLine("\nCurrentRegion for B7: " + currentRegion2.Address);
            Console.WriteLine("Row count in region: " + currentRegion2.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion2.ColumnCount);

            // Примените форматирование ко всему текущему региону
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            currentRegion1.SetStyle(style);

            // Сохраните книгу
            workbook.Save("RangePropertyCurrentRegionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


