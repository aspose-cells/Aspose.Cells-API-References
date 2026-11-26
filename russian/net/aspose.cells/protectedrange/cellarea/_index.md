---
title: "ProtectedRange.CellArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ProtectedRange. Возвращает объект CellArea, представляющий область ячеек, которую нужно защитить"
type: docs
url: /ru/net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

Возвращает объект `CellArea`, представляющий область ячеек, которую нужно защитить.

```csharp
public CellArea CellArea { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте защищённые диапазоны
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
            
            // Добавьте первый защищённый диапазон
            int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
            ProtectedRange range1 = allowRanges[index1];
            range1.Password = "123";

            // Добавьте второй защищённый диапазон
            int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
            ProtectedRange range2 = allowRanges[index2];
            range2.Password = "456";

            // Отобразите информацию о CellArea для обоих диапазонов
            Console.WriteLine("Protected Range 1:");
            Console.WriteLine($"Name: {range1.Name}");
            Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");

            Console.WriteLine("\nProtected Range 2:");
            Console.WriteLine($"Name: {range2.Name}");
            Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");

            // Сохраните книгу
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


