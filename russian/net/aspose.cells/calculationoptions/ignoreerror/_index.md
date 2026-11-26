---
title: "CalculationOptions.IgnoreError"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Указывает, следует ли игнорировать ошибки, возникшие при вычислении формул. Ошибка может быть связана с неподдерживаемой функцией, внешними ссылками и т.д. Значение по умолчанию — true."
type: docs
url: /ru/net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Указывает, следует ли игнорировать ошибки, возникшие при вычислении формул. Ошибка может быть вызвана неподдерживаемой функцией, внешними ссылками и т.д. Значение по умолчанию — true.

```csharp
public bool IgnoreError { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте именованный диапазон, которого не существует, чтобы продемонстрировать обработку ошибок
            worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
            
            // Вычислить с IgnoreError = false (будет выброшена ошибка)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
                Console.WriteLine("Calculation completed without ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (expected): " + ex.Message);
            }

            // Вычислить с IgnoreError = true (ошибка будет подавлена)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
                Console.WriteLine("Calculation completed while ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (unexpected): " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


