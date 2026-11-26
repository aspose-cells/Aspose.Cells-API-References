---
title: "ProtectedRange.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ProtectedRange. Возвращает название диапазона. Используется как дескриптор, а не как определение именованного диапазона"
type: docs
url: /ru/net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

Получает заголовок диапазона. Он используется как дескриптор, а не как определение именованного диапазона.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию защищённых диапазонов
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Добавить защищённый диапазон с именем "MyRange"
            int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];
            protectedRange.Password = "123";

            // Получить доступ и отобразить свойство Name
            Console.WriteLine("Protected range name: " + protectedRange.Name);
            Console.WriteLine("Cell area: {0},{1} to {2},{3}", 
                protectedRange.CellArea.StartRow,
                protectedRange.CellArea.StartColumn,
                protectedRange.CellArea.EndRow,
                protectedRange.CellArea.EndColumn);

            // Добавить ещё один именованный диапазон
            index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
            ProtectedRange secondRange = allowRanges[index];
            Console.WriteLine("Second protected range name: " + secondRange.Name);

            // Сохраните книгу
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


