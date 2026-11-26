---
title: "AutoFilter.FilterColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFilter. Возвращает коллекцию столбцов фильтра"
type: docs
url: /ru/net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Получает коллекцию столбцов фильтра.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyFilterColumnsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Status");
            
            worksheet.Cells["A2"].PutValue("HR");
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["C2"].PutValue("Present");
            
            worksheet.Cells["A3"].PutValue("IT");
            worksheet.Cells["B3"].PutValue("Sarah");
            worksheet.Cells["C3"].PutValue("Absent");
            
            worksheet.Cells["A4"].PutValue("HR");
            worksheet.Cells["B4"].PutValue("Mike");
            worksheet.Cells["C4"].PutValue("Present");

            // Применить автофильтр
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:C1";
            
            // Фильтровать столбец 2 (Status) по значениям "Present"
            autoFilter.Filter(2, "Present");
            
            // Получить доступ к столбцу фильтра
            FilterColumn filterColumn = autoFilter.FilterColumns[2];
            
            // Сохраните книгу
            workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


