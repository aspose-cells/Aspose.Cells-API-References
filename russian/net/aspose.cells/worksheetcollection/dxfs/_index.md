---
title: "WorksheetCollection.Dxfs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorksheetCollection свойство. Получает основные записи дифференциального форматирования"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/dxfs/
---
## WorksheetCollection.Dxfs property

Получает записи главного дифференциального форматирования.

```csharp
public DxfCollection Dxfs { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyDxfsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Установить условие и стиль
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            fcc[0].Style = style;
            
            // Продемонстрировать свойство Dxfs
            Console.WriteLine("Dxfs count before applying formatting: " + workbook.Worksheets.Dxfs.Count);
            
            // Применить форматирование, которое будет добавлено в Dxfs
            worksheet.ConditionalFormattings[0][0].Priority = 1;
            
            Console.WriteLine("Dxfs count after applying formatting: " + workbook.Worksheets.Dxfs.Count);
        }
    }
}
```

### См. также

* class [DxfCollection](../../dxfcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


