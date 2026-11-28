---
title: "TxtSaveOptions.Encoding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Varsayılan kodlamayı alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/encoding/
---
## TxtSaveOptions.Encoding property

Varsayılan kodlamayı alır ve ayarlar.

```csharp
public Encoding Encoding { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            
            // ASCII kodlamasıyla TXT kaydetme seçenekleri oluşturun
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = '\t'
            };
            
            // Çalışma kitabını belirtilen kodlamayla kaydedin
            workbook.Save("output.txt", saveOptions);
            
            Console.WriteLine("File saved with ASCII encoding");
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


