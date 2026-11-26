---
title: "HtmlSaveOptions.SaveAsSingleFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, сохранять ли HTML в один файл. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

Указывает, сохранять ли HTML как один файл. Значение по умолчанию — false.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### Примечания

Если в книге несколько листов или других необходимых ресурсов, таких как изображения, обычно эти листы и ресурсы нужно сохранять в отдельные файлы. В некоторых сценариях пользователю может потребоваться один итоговый файл для удобства передачи. В этом случае пользователь может установить это свойство в значение true.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Инициализировать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportPageHeaders = true;
            
            // Сохранить книгу в один HTML‑файл
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            // Проверьте, что выходной файл существует
            if (File.Exists(outputPath))
            {
                Console.WriteLine("HTML saved as single file successfully.");
            }
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


