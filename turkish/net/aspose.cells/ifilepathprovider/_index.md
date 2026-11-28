---
title: "Arayüz IFilePathProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.IFilePathProvider arayüzü. Dışa aktarılan dosya yolu sağlayıcısını temsil eder"
type: docs
url: /tr/net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

Dışa aktarılan dosya yolu sağlayıcısını temsil eder.

```csharp
public interface IFilePathProvider
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | Çalışma Sayfasını ayrı ayrı HTML olarak dışa aktarırken, dosyanın tam yolunu Çalışma Sayfası adıyla alır. Böylece Çalışma Sayfaları arasındaki referanslar doğru şekilde dışa aktarılabilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // IFilePathProvider arayüzündeki GetFullName metodunu uygulama
        public string GetFullName(string sheetName)
        {
            // Demonstrasyon amacıyla, sayfa adına dayalı basit bir dosya yolu döndür
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // Yeni bir çalışma kitabı oluştur ve bazı veriler ekle
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // HtmlSaveOptions oluştur ve FilePathProvider'ı ayarla
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Çalışma kitabını HTML formatında kaydedin
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


