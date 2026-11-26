---
title: "ProtectedRange.GetAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ProtectedRange. Возвращает все связанные области"
type: docs
url: /ru/net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

Получает все ссылочные области.

```csharp
public CellArea[] GetAreas()
```

### Возвращаемое значение

Возвращает все связанные области.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeMethodGetAreasDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить коллекцию защищённых диапазонов
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Добавить защищённый диапазон
            int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Получить области защищённого диапазона
            CellArea[] areas = protectedRange.GetAreas();
            
            // Вывести количество областей (должно быть 1 для этого простого диапазона)
            Console.WriteLine("Number of areas in protected range: " + areas.Length);
            
            // Сохраните книгу
            workbook.Save("ProtectedRangeExample.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


