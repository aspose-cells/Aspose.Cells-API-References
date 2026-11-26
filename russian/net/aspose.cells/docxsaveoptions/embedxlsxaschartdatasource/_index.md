---
title: "DocxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocxSaveOptions. Указывает, встраивается ли файл xlsx в качестве источника данных диаграммы"
type: docs
url: /ru/net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

Указывает, встраивается ли файл xlsx в качестве источника данных диаграммы.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // Инициализируйте DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Отобразить значение свойства EmbedXlsxAsChartDataSource по умолчанию
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Установите EmbedXlsxAsChartDataSource в true, чтобы продемонстрировать его использование
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Сохраните книгу в формате DOCX с настроенными параметрами
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with EmbedXlsxAsChartDataSource option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


