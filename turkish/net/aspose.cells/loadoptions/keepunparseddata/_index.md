---
title: "LoadOptions.KeepUnparsedData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirler. Varsayılan değer true'tur"
type: docs
url: /tr/net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Şablon dosyasından yüklendiğinde Çalışma kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirler. Varsayılan değer doğrudur.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Açıklamalar

Kullanıcının yalnızca şablon dosyasından bazı içerikleri okuması gerektiği ve çalışma kitabını geri kaydetmeye ihtiyaç duymadığı senaryolar için, bu özelliği false olarak ayarlamak performansı artırabilir, özellikle bir tür LoadFilter ile birlikte kullanıldığında,

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyKeepUnparsedDataDemo
    {
        public static void Run()
        {
            // Yükleme seçeneklerini oluşturun ve KeepUnparsedData'yı false olarak ayarlayın
            LoadOptions options = new LoadOptions();
            options.KeepUnparsedData = false;

            // Seçeneklerle çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsx", options);

            // Çalışma sayfasına erişin ve ayrıştırılmamış verilerin tutulmadığını gösterin
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


