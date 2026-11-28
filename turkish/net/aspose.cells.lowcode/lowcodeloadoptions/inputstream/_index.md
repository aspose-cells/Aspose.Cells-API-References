---
title: "LowCodeLoadOptions.InputStream"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeLoadOptions özelliği. Şablonun akışını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

Şablonun akışını alır ve ayarlar.

```csharp
public Stream InputStream { get; set; }
```

### Açıklamalar

Bu özelliğe null olmayan bir Stream ayarlandığında, daha önce ayarlanan [`InputFile`](../inputfile/) değeri göz ardı edilecektir.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeLoadOptionsPropertyInputStreamDemo
    {
        public static void Run()
        {
            // Bellek akışında örnek veri oluşturun
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // InputStream ile yükleme seçenekleri oluşturun
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // Akışı kullanarak yeni bir çalışma kitabı oluşturun
                using (Workbook workbook = new Workbook(stream))
                {
                    // İlk çalışma sayfasına eriş
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // İçeriğin yüklendiğini gösterin
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


