---
title: "TxtLoadOptions.TextQualifier"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Hücre değerleri için metin niteleyicisini belirtir. Varsayılan niteleyici"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

Hücre değerleri için metin niteleyicisini belirtir. Varsayılan niteleyici '\"' dir.

```csharp
public char TextQualifier { get; set; }
```

### Açıklamalar

Bu özellik ayarlandığında, [`HasTextQualifier`](../hastextqualifier/) otomatik olarak doğru (true) olacaktır.

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTextQualifierDemo
    {
        public static void Run()
        {
            // CSV için bir TxtLoadOptions örneği oluşturun
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Metin niteleyicileriyle örnek CSV verisi oluşturun
            string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
            
            // Örnek veriyi geçici bir dosyaya kaydedin
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvData);

            // Belirtilen seçeneklerle CSV dosyasını yükleyin
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("TextQualifierDemo.xlsx");

            // Geçici dosyayı temizleyin
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


