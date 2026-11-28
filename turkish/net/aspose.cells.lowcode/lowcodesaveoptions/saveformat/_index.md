---
title: "LowCodeSaveOptions.SaveFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptions özelliği. Çıktı için kaydetme formatını alır ve ayarlar. Genel olarak düşük kod yöntemiyle belirli bir işlem için yalnızca bazı belirli formatlara izin verilir. Lütfen ilgili işlem için doğru formatı belirtin; aksi takdirde beklenmeyen sonuçlar veya hatta istisna oluşabilir."
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptions/saveformat/
---
## LowCodeSaveOptions.SaveFormat property

Çıktı için kaydetme formatını alır ve ayarlar. Genel olarak, düşük kod yöntemiyle belirli bir işlem için yalnızca bazı belirli formatlara izin verilir. Lütfen ilgili işlem için doğru formatı belirtin, aksi takdirde beklenmeyen sonuçlar veya hatta istisna oluşabilir.

```csharp
public virtual SaveFormat SaveFormat { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // LowCodeSaveOptions'ı farklı formatlarla başlatın
            LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
            LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();

            // Excel kaydetme seçeneklerini yapılandırın
            excelOptions.SaveFormat = SaveFormat.Xlsx;
            excelOptions.OutputFile = "output_excel.xlsx";

            // PDF kaydetme seçeneklerini yapılandırın
            pdfOptions.SaveFormat = SaveFormat.Pdf;
            pdfOptions.OutputFile = "output_pdf.pdf";

            // Orijinal formatta kaydetmeyi gösterin
            Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
            workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);

            // Format değişikliğini ve yeniden kaydetmeyi gösterin
            Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
            Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
            workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);

            Console.WriteLine("Files saved successfully with different formats.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


