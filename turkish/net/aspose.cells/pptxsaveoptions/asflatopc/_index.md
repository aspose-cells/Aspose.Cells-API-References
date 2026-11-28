---
title: "PptxSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PptxSaveOptions özelliği. Open XML SDK tarafından oluşturulabilen düz bir opc dosyası olarak kaydedilip kaydedilmediğini gösterir."
type: docs
url: /tr/net/aspose.cells/pptxsaveoptions/asflatopc/
---
## PptxSaveOptions.AsFlatOpc property

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

    public class PptxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Flat OPC Demo";

            try
            {
                // PptxSaveOptions örneği oluşturun
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // AsFlatOpc'un varsayılan değerini gösterin
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Özelliği true olarak ayarlayarak kullanımını gösterin
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Seçenek etkinleştirilmiş şekilde çalışma kitabını PPTX olarak kaydedin
                workbook.Save("AsFlatOpcDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with AsFlatOpc enabled");
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

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


