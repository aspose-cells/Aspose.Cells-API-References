---
title: "Worksheet.IsSelected"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, выбран ли этот лист при открытии книги"
type: docs
url: /ru/net/aspose.cells/worksheet/isselected/
---
## Worksheet.IsSelected property

Указывает, выбран ли этот лист при открытии книги.

```csharp
public bool IsSelected { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить второй лист
            workbook.Worksheets.Add("Sheet2");
            
            // Получить первый лист
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "FirstSheet";
            
            // Получить второй лист
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet2.Name = "SecondSheet";
            
            // Продемонстрировать свойство IsSelected
            Console.WriteLine("Before selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Выбрать второй лист
            worksheet2.IsSelected = true;
            workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
            
            Console.WriteLine("\nAfter selection:");
            Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
            Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
            
            // Сохраните книгу
            workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


