---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор HtmlSaveOptions. Создаёт параметры для сохранения html‑файла"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions() {#constructor}

Создаёт параметры для сохранения HTML‑файла.

```csharp
public HtmlSaveOptions()
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Инициализировать HtmlSaveOptions с помощью конструктора
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Сохранить как HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved to: " + outputPath);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlSaveOptions(SaveFormat) {#constructor_1}

Создаёт параметры для сохранения HTM‑файла.

```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат файла. Он должен быть одним из следующих типов: Html или MHtml, иначе сохранённый формат будет автоматически установлен как Html. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            try
            {
                // Создайте HtmlSaveOptions с параметром SaveFormat
                HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
                
                // Установите некоторые свойства
                saveOptions.PageTitle = "Aspose.Cells HTML Export";
                saveOptions.ExportActiveWorksheetOnly = true;
                saveOptions.ExportGridLines = true;
                
                // Сохраните книгу с помощью HtmlSaveOptions
                workbook.Save("HtmlExportWithOptions.html", saveOptions);
                
                Console.WriteLine("HTML file saved successfully with HtmlSaveOptions(SaveFormat)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HtmlSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


