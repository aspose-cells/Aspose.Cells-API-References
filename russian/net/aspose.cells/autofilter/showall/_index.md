---
title: "AutoFilter.ShowAll"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Отображает все строки"
type: docs
url: /ru/net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

Отобразить все скрытые строки.

```csharp
public void ShowAll()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodShowAllDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Фильтр, показывающий только "Apple"
            worksheet.AutoFilter.Filter(0, "Apple");
            
            // Снова показать все данные
            worksheet.AutoFilter.ShowAll();
            
            // Сохраните книгу
            workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


