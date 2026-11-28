---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DbfSaveOptions yapıcı. .dbf dosyasını kaydetme seçenekleri"
type: docs
url: /tr/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

.dbf dosyasını kaydetme seçenekleri.

```csharp
public DbfSaveOptions()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Yapıcıyı kullanarak DbfSaveOptions örneği oluştur
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // Kaydetme seçeneklerinin özelliklerini ayarla
                saveOptions.ExportAsString = true;
                
                // Çalışma kitabını DBF kaydetme seçenekleriyle kaydedin
                workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
                
                Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving DBF file: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


