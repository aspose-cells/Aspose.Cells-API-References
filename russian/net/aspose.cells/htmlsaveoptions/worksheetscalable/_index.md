---
title: "HtmlSaveOptions.WorksheetScalable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, происходит ли масштабирование HTML через уровень масштабирования листа при сохранении файла в HTML; значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Указывает, следует ли масштабировать HTML с помощью уровня масштабирования листа при сохранении файла в HTML, значение по умолчанию — false.

```csharp
public bool WorksheetScalable { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWorksheetScalableDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Установить параметры сохранения HTML с свойством WorksheetScalable
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            
            // Сохранить рабочую книгу с параметрами HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, options);
            
            // Проверьте, что вывод содержит стиль масштабирования
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


