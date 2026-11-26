---
title: "Workbook.Worksheets"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает коллекцию WorksheetCollection в электронной таблице"
type: docs
url: /ru/net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Получает коллекцию [`WorksheetCollection`](../../worksheetcollection/) в электронной таблице.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Возвращаемое значение

[`WorksheetCollection`](../../worksheetcollection/) collection

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyWorksheetsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Добавить новый лист
            workbook.Worksheets.Add("SecondSheet");
            
            // Получить доступ ко второму листу и добавить данные
            Worksheet secondSheet = workbook.Worksheets[1];
            secondSheet.Cells["A1"].PutValue("Product");
            secondSheet.Cells["B1"].PutValue("Price");
            secondSheet.Cells["A2"].PutValue("Laptop");
            secondSheet.Cells["B2"].PutValue(999.99);
            
            // Сохраните книгу
            workbook.Save("WorkbookWorksheetsDemo.xlsx");
            
            // Вывести количество листов
            Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


