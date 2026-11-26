---
title: "HtmlSaveOptions.CalculateFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, следует ли вычислять формулы перед сохранением HTML‑файла"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/calculateformula/
---
## HtmlSaveOptions.CalculateFormula property

Указывает, следует ли вычислять формулы перед сохранением HTML‑файла.

```csharp
public bool CalculateFormula { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте данные и формулы в лист
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Создайте HtmlSaveOptions с установленным CalculateFormula в true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                CalculateFormula = true
            };

            // Сохраните книгу в формате HTML — формулы будут вычислены
            workbook.Save("HtmlWithCalculatedFormulas.html", saveOptions);

            Console.WriteLine("HTML file with calculated formulas created successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


