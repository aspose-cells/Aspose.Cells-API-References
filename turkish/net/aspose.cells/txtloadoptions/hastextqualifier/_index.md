---
title: "TxtLoadOptions.HasTextQualifier"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Hücre değeri için metin niteleyicisinin olup olmadığı. Varsayılan true'tur"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

Hücre değeri için metin niteleyicisinin olup olmadığı. Varsayılan değer true'tur.

```csharp
public bool HasTextQualifier { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasTextQualifierDemo
    {
        public static void Run()
        {
            // Metin niteleyicileriyle CSV içeriği oluşturun
            string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
            
            // CSV içeriğini geçici bir dosyaya kaydedin
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);

            // HasTextQualifier true olarak ayarlanmış TxtLoadOptions oluşturun
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Metin niteleyicileriyle CSV dosyasını yükleyin
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Başarılı yüklemeyi göstermek için çalışma kitabını kaydedin
            workbook.Save("Output.xlsx");

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


