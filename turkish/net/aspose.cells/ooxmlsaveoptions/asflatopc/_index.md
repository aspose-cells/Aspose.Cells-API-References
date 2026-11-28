---
title: "OoxmlSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OoxmlSaveOptions özelliği. Açık XML SDK tarafından oluşturulabilen düz opc dosyası olarak kaydedilip kaydedilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/ooxmlsaveoptions/asflatopc/
---
## OoxmlSaveOptions.AsFlatOpc property

Open XML SDK tarafından oluşturulabilen düz opc dosyası olarak kaydedilip kaydedilmeyeceğini gösterir.

```csharp
public bool AsFlatOpc { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Flat OPC Demo");

            try
            {
                // OoxmlSaveOptions örneği oluşturun
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // AsFlatOpc özelliğinin varsayılan değerini gösterin
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // AsFlatOpc'ı true olarak ayarlayın
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // AsFlatOpc etkinleştirilmiş halde çalışma kitabını kaydedin
                workbook.Save("AsFlatOpc_Enabled.xlsx", saveOptions);

                // AsFlatOpc devre dışı bırakılmış başka bir kaydetme seçeneği oluşturun
                OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
                saveOptions2.AsFlatOpc = false;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions2.AsFlatOpc);

                // AsFlatOpc devre dışı bırakılmış halde çalışma kitabını kaydedin
                workbook.Save("AsFlatOpc_Disabled.xlsx", saveOptions2);

                Console.WriteLine("AsFlatOpc property demonstration completed successfully.");
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

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


