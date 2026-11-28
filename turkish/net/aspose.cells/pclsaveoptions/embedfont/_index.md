---
title: "PclSaveOptions.EmbedFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PclSaveOptions özelliği. Yazı tipinin çıktı Pcl dosyasına gömülüp gömülmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

Çıktı Pcl dosyasına yazı tipinin gömülüp gömülmeyeceğini belirtir.

```csharp
public bool EmbedFont { get; set; }
```

### Açıklamalar

Varsayılan değer true'tur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve bazı örnek veriler ekleyin
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // PCL kaydetme seçenekleri oluşturun
                PclSaveOptions pclOptions = new PclSaveOptions();

                // EmbedFont özelliğinin mevcut değerini okuyun ve görüntüleyin
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (İsteğe bağlı) Özellik yazılabilir ise ayarlayabilirsiniz, ancak burada sadece okuyoruz
                // pclOptions.EmbedFont = true;

                // Seçenekleri kullanarak çalışma kitabını bir PCL dosyası olarak kaydedin
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


