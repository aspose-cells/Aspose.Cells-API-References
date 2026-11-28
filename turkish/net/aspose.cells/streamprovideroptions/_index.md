---
title: "Sınıf StreamProviderOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.StreamProviderOptions sınıfı. Akış seçeneklerini temsil eder."
type: docs
url: /tr/net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

Akış seçeneklerini temsil eder.

```csharp
public class StreamProviderOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Yeni bir `StreamProviderOptions` sınıfı örneği başlatır. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Yeni bir `StreamProviderOptions` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | Kullanıcının özelleştirilmiş yolu (URL), başvurulan kaynak için oluşturulan html dosyasında kaydedilir. Kullanıcı tarafından tanımlanmazsa, DefaultPath kullanılacaktır. Örneğin, sayfa verileri kullanıcı tarafından d:/sheet001.htm konumuna kaydedilecek, ana html dosyasında kullanılan url "d:/sheet001.htm" ya da ana html dosyası tarafından erişilebilen başka geçerli bir göreli yol olmalıdır. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | Üretilen html dosyasında başvurulan kaynak için kaydedilen varsayılan yol(URL). Örneğin, sayfa verileri xxx_files/sheet001.htm içinde kaydedildiğinde, ana html dosyasında kullanılan url şu şekilde olmalıdır "src=\"xxx_files/sheet001.htm\"" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Yükleme kaynağının tipini alır ve ayarlar. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Akışı alır/ayarlar. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassStreamProviderOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // StreamProviderOptions oluştur.
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Demonstrasyon için bir bellek akışı ayarla.
            options.Stream = new MemoryStream();
            
            // Akışı kullan (örnek: çalışma kitabını akışa kaydet).
            workbook.Save(options.Stream, SaveFormat.Xlsx);
            
            // Akışı kapatmayı göster.
            CloseStream(options);
        }

        public static void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


