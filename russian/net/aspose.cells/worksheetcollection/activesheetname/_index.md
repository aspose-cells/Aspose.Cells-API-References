---
title: "WorksheetCollection.ActiveSheetName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Представляет имя активного листа при открытии таблицы"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Представляет имя активного листа при открытии таблицы.

```csharp
public string ActiveSheetName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько листов
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Установить активный лист по имени
            workbook.Worksheets.ActiveSheetName = "Sheet2";

            // Проверить активный лист
            Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);

            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


