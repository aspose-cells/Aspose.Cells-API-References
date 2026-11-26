---
title: "WorksheetCollection.ActiveSheetIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Представляет индекс активного листа при открытии таблицы"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Представляет индекс активного листа при открытии таблицы.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Примечания

Индекс листа начинается с нуля.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу с 3 листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Установить индекс активного листа в 1 (второй лист)
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Проверить активный лист
            Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);

            // Сохраните книгу
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
            workbook.Save(outputPath);

            Console.WriteLine("File saved to: " + outputPath);
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


