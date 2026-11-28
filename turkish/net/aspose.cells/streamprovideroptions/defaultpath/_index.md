---
title: "StreamProviderOptions.DefaultPath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StreamProviderOptions özelliği. Başvurulan kaynak için oluşturulan html dosyasında kaydedilen varsayılan pathURL. Örneğin, sayfa verileri xxx_files/sheet001.htm içinde kaydedildiğinde, ana html dosyasında kullanılan url srcxxx_files/sheet001.htm gibi olmalıdır."
type: docs
url: /tr/net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

Üretilen html dosyasında başvurulan kaynak için kaydedilen varsayılan yol(URL). Örneğin, sayfa verileri xxx_files/sheet001.htm içinde kaydedildiğinde, ana html dosyasında kullanılan url şu şekilde olmalıdır "src=\"xxx_files/sheet001.htm\""

```csharp
public string DefaultPath { get; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyDefaultPathDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();
            
            // ResourceLoadingType ve DefaultPath ile StreamProviderOptions oluşturun
            StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
            
            // DefaultPath kullanımını gösterin
            Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
            
            // Seçenekleri bir akışla kullanma örneği (basitleştirilmiş gösterim)
            using (MemoryStream stream = new MemoryStream())
            {
                options.Stream = stream;
                
                if (options.DefaultPath.IndexOf("1.") >= 0)
                {
                    Console.WriteLine("Processing stream for path: " + options.DefaultPath);
                    // Akış ile işlemler gerçekleştirin
                    workbook.Save(stream, SaveFormat.Xlsx);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


