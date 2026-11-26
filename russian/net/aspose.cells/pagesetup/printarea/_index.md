---
title: "PageSetup.PrintArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет диапазон для печати"
type: docs
url: /ru/net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Представляет диапазон для печати.

```csharp
public string PrintArea { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(3);
            
            // Установить область печати A1:B3
            worksheet.PageSetup.PrintArea = "A1:B3";
            
            // Сохранить только с областью печати
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportPrintAreaOnly = true
            };
            
            workbook.Save("PrintAreaDemo.html", options);
            
            Console.WriteLine("Print area demo created successfully.");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


