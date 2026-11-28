---
title: "TxtSaveOptions.Separator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Metin dosyasının karakter sınırlayıcısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

Metin dosyasının karakter sınırlayıcısını alır ve ayarlar.

```csharp
public char Separator { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Virgül ayırıcı ile TXT kaydetme seçeneklerini yapılandır
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.Separator = ',';
            txtSaveOptions.Encoding = System.Text.Encoding.UTF8;

            // Çalışma kitabını virgül ayırıcı ile CSV olarak kaydet
            string outputPath = "output.csv";
            workbook.Save(outputPath, txtSaveOptions);

            // Kaydedilen dosya içeriğini göster
            Console.WriteLine("File saved with comma separator:");
            Console.WriteLine(File.ReadAllText(outputPath));
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


