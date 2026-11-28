---
title: "DocxSaveOptions.AsNormalView"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocxSaveOptions özelliği. Excel dosyasını normal görünümde docx dosyasına dışa aktarır. Bu özellik true ise bir Alan çıktılanır ve ölçek etkili olmaz. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

Excel dosyasını normal görünümde docx dosyasına dışa aktarma. Bu özellik true ise, bir Area çıktılanacak ve ölçek etkili olmayacak. Varsayılan değer false.

```csharp
public bool AsNormalView { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına erişin ve örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // DocxSaveOptions'ı başlatın
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // AsNormalView özelliğinin varsayılan değerini göster
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // Kullanımını göstermek için AsNormalView'ı true olarak ayarla
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // Çalışma kitabını yapılandırılmış seçeneklerle DOCX olarak kaydedin
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


