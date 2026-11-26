---
title: "Cell.Worksheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает родительский рабочий лист"
type: docs
url: /ru/net/aspose.cells/cell/worksheet/
---
## Cell.Worksheet property

Получает родительский лист.

```csharp
public Worksheet Worksheet { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Получите доступ к ячейке и продемонстрируйте свойство Worksheet
            Cell cell = worksheet.Cells["A3"];
            
            // Отобразите информацию о рабочем листе через свойство Worksheet ячейки
            Console.WriteLine("Cell A3 is in worksheet: " + cell.Worksheet.Name);
            Console.WriteLine("Calculation result in A3: " + cell.Value);
            
            // Добавьте еще один рабочий лист и продемонстрируйте перекрестную ссылку
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=A3");
            
            // Получите доступ к ячейке в Sheet2 и покажите её рабочий лист
            Cell crossSheetCell = sheet2.Cells["B1"];
            Console.WriteLine("Cell B1 is in worksheet: " + crossSheetCell.Worksheet.Name);
            Console.WriteLine("Cross-sheet reference in B1: " + crossSheetCell.Value);
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


