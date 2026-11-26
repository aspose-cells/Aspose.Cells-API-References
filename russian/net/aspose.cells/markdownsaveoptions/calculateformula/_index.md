---
title: "MarkdownSaveOptions.CalculateFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MarkdownSaveOptions свойство. Указывает, следует ли вычислять формулы перед сохранением markdown‑файла"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

Указывает, следует ли вычислять формулы перед сохранением markdown-файла.

```csharp
public bool CalculateFormula { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные с формулами
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // Создайте экземпляр MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Отобразите значение CalculateFormula по умолчанию
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // Установите CalculateFormula в true, чтобы вычислять формулы перед сохранением
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Сохраните книгу с включённым вычислением формул
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // Установите CalculateFormula в false, чтобы сохранять формулы без изменений
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Сохраните книгу с отключённым вычислением формул
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


