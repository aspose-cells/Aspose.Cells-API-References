---
title: "Worksheet.IsRowColumnHeadersVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает или задает значение, указывающее, будет ли лист отображать заголовки строк и столбцов. По умолчанию true"
type: docs
url: /ru/net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

Получает или задаёт значение, указывающее, будет ли лист отображать заголовки строк и столбцов. По умолчанию true.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить видимость заголовков строк и столбцов в false
            worksheet.IsRowColumnHeadersVisible = false;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Загрузить сохранённую книгу, чтобы проверить свойство
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Вывести значение свойства
            Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


