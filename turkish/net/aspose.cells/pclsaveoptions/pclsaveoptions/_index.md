---
title: "PclSaveOptions.PclSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PclSaveOptions yapıcı. PCL dosyası kaydetmek için seçenekleri oluşturur"
type: docs
url: /tr/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

Pcl dosyası kaydetme seçeneklerini oluşturur.

```csharp
public PclSaveOptions()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // #ctor yöntemini çağırarak PclSaveOptions örneği oluşturun
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // Gerekirse ek seçenekleri yapılandırın
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // Çalışma kitabını PCL seçenekleriyle kaydedin
                workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


