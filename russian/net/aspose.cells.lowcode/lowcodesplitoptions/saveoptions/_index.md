---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSplitOptions. Параметры сохранения для сохранения разделённых частей"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

Параметры сохранения для сохранения разделённых частей.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу и добавить примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Создайте экземпляр LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Отобразить начальное значение SaveOptions (по умолчанию null)
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // Создать и настроить LowCodeSaveOptions для формата PDF
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // Назначить параметры сохранения объекту SplitOptions
            splitOptions.SaveOptions = pdfSaveOptions;

            // Отобразить обновлённое значение SaveOptions
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // Пример сценария использования: При разделении книги части будут сохраняться в формате PDF
            // (Фактический код разделения будет зависеть от реализации API Aspose.Cells.LowCode)
            // LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
            
            // Сохраните оригинальную книгу для демонстрации (не затронутую SplitOptions)
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


