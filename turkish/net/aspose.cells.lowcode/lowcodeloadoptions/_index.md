---
title: "LowCodeLoadOptions sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodeLoadOptions sınıfı. Şablon dosyasını yüklemek için seçenekler"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

Şablon dosyasını yükleme seçenekleri.

```csharp
public class LowCodeLoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Şablonun dosyasını (gerekirse yol ile) alır ve ayarlar. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Şablonun akışını alır ve ayarlar. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // Örnek bir akış oluşturun (demo amaçlı bellek içi)
            using (MemoryStream stream = new MemoryStream())
            {
                // Yeni bir çalışma kitabı oluşturun ve demo için akışa kaydedin
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // Akış konumunu sıfırlayın
                stream.Position = 0;

                // LowCodeLoadOptions oluşturun ve kullanın
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // Örnek kullanım - genellikle bir işleme yöntemine geçirilir
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


