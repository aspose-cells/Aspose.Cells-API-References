---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfPlaceHolders. Шаблон для создания экземпляра параметров сохранения в GetSaveOptions"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate property

Шаблон для создания экземпляра параметров сохранения в [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Примечания

Если шаблон был указан, созданный экземпляр скопирует все настройки из него и соответственно обновит выходной файл.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            
            // Инициализировать провайдер с шаблоном пути, содержащим заполнители
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/Sheet_{sheet}_Part_{part}.pdf");
            
            // Отобразить начальное состояние шаблона
            Console.WriteLine($"Initial SaveOptionsTemplate: {(provider.SaveOptionsTemplate == null ? "Not set" : "Configured")}");
            
            // Создать и настроить новый шаблон параметров сохранения
            provider.SaveOptionsTemplate = new LowCodePdfSaveOptions
            {
                PdfOptions = new PdfSaveOptions  // Fixed property name from PdfSaveOptions to PdfOptions
                {
                    Compliance = PdfCompliance.PdfA1a,
                    ExportDocumentStructure = true
                }
            };

            // Настроить параметры разбиения
            provider.BuildPathWithSheetAlways = true;
            provider.SplitPartPrefix = "Split_";
            
            // Отобразить настроенные параметры PDF
            var pdfOptions = (LowCodePdfSaveOptions)provider.SaveOptionsTemplate;
            Console.WriteLine($"Configured PDF Compliance: {pdfOptions.PdfOptions.Compliance}");  // Fixed property access
            Console.WriteLine($"Document Structure Export: {pdfOptions.PdfOptions.ExportDocumentStructure}");  // Fixed property access

            // Добавить разрыв страницы для создания частей разбиения
            worksheet.HorizontalPageBreaks.Add(0);
            
            // Сохранить, используя конфигурацию провайдера (здесь произойдёт фактическое разбиение/сохранение)
            Console.WriteLine("Workbook prepared with SaveOptionsTemplate configuration");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


