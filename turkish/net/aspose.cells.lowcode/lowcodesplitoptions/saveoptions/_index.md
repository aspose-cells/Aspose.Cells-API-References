---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSplitOptions özelliği. Bölünmüş parçaları kaydetmek için kaydetme seçenekleri"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

Bölünmüş parçaları kaydetmek için kaydetme seçenekleri.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve örnek veri ekle
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // LowCodeSplitOptions sınıfının bir örneğini oluşturun
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // İlk SaveOptions değerini göster (varsayılan olarak null)
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // PDF formatı için LowCodeSaveOptions oluştur ve yapılandır
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // Kaydetme seçeneklerini SplitOptions'a ata
            splitOptions.SaveOptions = pdfSaveOptions;

            // Güncellenmiş SaveOptions değerini göster
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // Örnek kullanım senaryosu: Çalışma kitabını bölmek, parçaları PDF olarak kaydeder
            // (Gerçek bölme kodu, Aspose.Cells.LowCode API uygulamasına bağlı olacaktır)
            // LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
            
            // Demonstrasyon için orijinal çalışma kitabını kaydedin (SplitOptions tarafından etkilenmez)
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


