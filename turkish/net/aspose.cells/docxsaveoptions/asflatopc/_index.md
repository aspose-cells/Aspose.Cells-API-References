---
title: "DocxSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocxSaveOptions özelliği. Açık XML SDK tarafından oluşturulabilen düz opc dosyası olarak kaydedilip kaydedilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/docxsaveoptions/asflatopc/
---
## DocxSaveOptions.AsFlatOpc property

Open XML SDK tarafından oluşturulabilen düz opc dosyası olarak kaydedilip kaydedilmediğini gösterir

```csharp
public bool AsFlatOpc { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına erişin ve örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Flat OPC Demo";

            try
            {
                // DocxSaveOptions'ı başlatın
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // AsFlatOpc özelliğinin varsayılan değerini gösterin
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Kullanımını göstermek için AsFlatOpc'i true olarak ayarlayın
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Çalışma kitabını yapılandırılmış seçeneklerle DOCX olarak kaydedin
                workbook.Save("AsFlatOpcDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsFlatOpc option.");
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


