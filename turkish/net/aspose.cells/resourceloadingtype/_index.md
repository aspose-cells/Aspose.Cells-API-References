---
title: "Enum ResourceLoadingType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ResourceLoadingType enum. Bağlı kaynağın nasıl yükleneceğini temsil eder"
type: docs
url: /tr/net/aspose.cells/resourceloadingtype/
---
## ResourceLoadingType enumeration

Bağlantılı kaynağın nasıl yükleneceğini temsil eder.

```csharp
public enum ResourceLoadingType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | Bu kaynağı her zamanki gibi yükler. |
| Skip | `1` | Bu kaynağın yüklenmesini atlar. |
| UserProvided | `2` | Kullanıcı tarafından sağlanan akışı kullan |

### Örnekler

```csharp
using Aspose.Cells;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ResourceLoadingTypeDemo
    {
        public static void ResourceLoadingTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Resource");
            worksheet.Cells["A2"].PutValue("Default");
            worksheet.Cells["A3"].PutValue("Skip");
            worksheet.Cells["A4"].PutValue("UserProvided");

            // Çalışma kitabını özel akış sağlayıcısı ile HTML olarak kaydet
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                StreamProvider = new CustomStreamProvider()
            };

            workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
        }
    }

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Kaynak için özel bir akış sağlayın
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Kaynağın yüklenmesini atla
                options.Stream = Stream.Null;
            }
            else
            {
                // Kaynağı normal şekilde yükle
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Akış null değilse kapat
            options.Stream?.Close();
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


