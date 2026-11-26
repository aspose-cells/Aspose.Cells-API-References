---
title: "LowCodeSaveOptions.SaveFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptions. Получает и задает формат сохранения для вывода. Обычно для конкретного процесса в low code режиме разрешены только некоторые форматы. Пожалуйста, укажите правильный формат для соответствующего процесса, иначе могут возникнуть неожиданные результаты или даже исключения."
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptions/saveformat/
---
## LowCodeSaveOptions.SaveFormat property

Получает и задает формат сохранения для вывода. Обычно для конкретного процесса в режиме низкого кода разрешены только определённые форматы. Пожалуйста, укажите правильный формат для соответствующего процесса, иначе могут возникнуть неожиданные результаты или даже исключения.

```csharp
public virtual SaveFormat SaveFormat { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Инициализировать LowCodeSaveOptions с разными форматами
            LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
            LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();

            // Настроить параметры сохранения Excel
            excelOptions.SaveFormat = SaveFormat.Xlsx;
            excelOptions.OutputFile = "output_excel.xlsx";

            // Настройте параметры сохранения PDF
            pdfOptions.SaveFormat = SaveFormat.Pdf;
            pdfOptions.OutputFile = "output_pdf.pdf";

            // Продемонстрировать сохранение в оригинальном формате
            Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
            workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);

            // Продемонстрировать изменение формата и повторное сохранение
            Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
            Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
            workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);

            Console.WriteLine("Files saved successfully with different formats.");
        }
    }
}
```

### См. также

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


