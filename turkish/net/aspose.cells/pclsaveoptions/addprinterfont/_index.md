---
title: "PclSaveOptions.AddPrinterFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PclSaveOptions yöntemi. Üretici tarafından yazıcıya zaten eklenmiş yazı tipi hakkında bilgi ekler"
type: docs
url: /tr/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

Üretici tarafından yazıcıya zaten eklenmiş yazı tipi hakkında bilgi ekler.

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFullName | String | Kaynak dosyada kullanılan yazı tipinin tam adı (örn. "Times New Roman Bold Italic"). |
| fontPclName | String | Çıktı Pcl belgesinde kullanılacak yazı tipinin adı. |

### Açıklamalar

Pcl spesifikasyonuna göre herhangi bir yazıcıda bulunması gereken 52 yazı tipi vardır. Ancak üreticiler cihazlarına başka yazı tipleri ekleyebilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yazı tipi kullanımını göstermek için çalışma sayfasına bazı metinler ekleyin
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // PCL kaydetme seçenekleri oluşturun
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // Belirli yazı tipi adlarıyla AddPrinterFont yöntemini çağırın
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // Çalışma kitabını PCL seçenekleriyle kaydedin
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


