---
title: "HtmlLoadOptions.HasFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Указывает, является ли текст формулой, если он начинается с"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Указывает, является ли текст формулой, если он начинается с "=".

```csharp
public bool HasFormula { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Установите HasFormula в false, чтобы рассматривать строковые формулы как обычный текст
            loadOptions.HasFormula = false;
            
            // Создать workbook с HTML‑файлом и параметрами загрузки
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Отобразить некоторые значения ячеек для демонстрации импорта HTML
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // Сохранить как XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


