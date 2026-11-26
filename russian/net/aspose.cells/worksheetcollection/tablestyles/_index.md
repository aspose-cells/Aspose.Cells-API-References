---
title: "WorksheetCollection.TableStyles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Получает объект TableStyles"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

Получает объект `TableStyles`.

```csharp
public TableStyleCollection TableStyles { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyTableStylesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько листов
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            // Создать и добавить стили таблиц
            int styleIndex1 = workbook.Worksheets.TableStyles.AddTableStyle("Style1");
            TableStyle style1 = workbook.Worksheets.TableStyles[styleIndex1];
            
            int styleIndex2 = workbook.Worksheets.TableStyles.AddTableStyle("Style2");
            TableStyle style2 = workbook.Worksheets.TableStyles[styleIndex2];
            
            // Отобразить количество стилей таблиц
            Console.WriteLine("Table styles count: " + workbook.Worksheets.TableStyles.Count);
            
            // Удалить один стиль
            workbook.Worksheets.TableStyles.RemoveAt(0);
            
            // Отобразить обновленное количество
            Console.WriteLine("Table styles count after removal: " + workbook.Worksheets.TableStyles.Count);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


