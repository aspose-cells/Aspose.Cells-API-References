---
title: "TxtLoadOptions.HasFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Указывает, является ли текст формулой, если он начинается с"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

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
    public class TxtLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки текста и включите разбор формул
            TxtLoadOptions options = new TxtLoadOptions();
            options.HasFormula = true;
            options.SeparatorString = "|";

            // Загрузите рабочую книгу с формулами из текстового файла
            Workbook workbook = new Workbook("example.csv", options);
            
            // Получите доступ к ячейке с формулой и отобразите её
            Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
            
            // Сохраните книгу
            workbook.Save("example_output.xlsx");
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


