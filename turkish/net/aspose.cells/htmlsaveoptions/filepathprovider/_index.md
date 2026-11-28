---
title: "HtmlSaveOptions.FilePathProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Worksheet'i ayrı ayrı HTML'e dışa aktarmak için IFilePathProvider'ı alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/filepathprovider/
---
## HtmlSaveOptions.FilePathProvider property

Çalışma sayfasını ayrı ayrı HTML'ye dışa aktarmak için IFilePathProvider'ı alır veya ayarlar.

```csharp
public IFilePathProvider FilePathProvider { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFilePathProviderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve bazı veriler ekle
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // HtmlSaveOptions oluştur ve FilePathProvider'ı ayarla
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new CustomFilePathProvider();

            // Çalışma kitabını HTML formatında kaydedin
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }

    public class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Dosya yolları oluşturmak için özel mantık
            return $"custom_{sheetName}";
        }
    }
}
```

### Ayrıca Bakınız

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


