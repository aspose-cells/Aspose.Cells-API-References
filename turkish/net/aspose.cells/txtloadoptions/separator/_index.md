---
title: "TxtLoadOptions.Separator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Metin dosyasının karakter ayıracısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/separator/
---
## TxtLoadOptions.Separator property

Metin dosyasının karakter ayırıcıyı alır ve ayarlar.

```csharp
public char Separator { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Örnek veri oluşturun ve özel ayırıcıyla kaydedin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = '*';
            workbook.Save("output.csv", saveOptions);

            // Kaydedilen dosyayı aynı ayırıcıyla yükleyin
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = '*';
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // Yüklenen veriyi doğrulayın
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


