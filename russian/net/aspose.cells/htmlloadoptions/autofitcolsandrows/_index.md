---
title: "HtmlLoadOptions.AutoFitColsAndRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Указывает, следует ли автоматически подгонять столбцы и строки. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Указывает, следует ли автоматически подгонять столбцы и строки. Значение по умолчанию — false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Включить автоматическую подгонку столбцов и строк
            loadOptions.AutoFitColsAndRows = true;
            
            // Загрузить HTML‑файл с указанными параметрами
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Автоподгонка столбцов и строк будет применена при загрузке
            Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


