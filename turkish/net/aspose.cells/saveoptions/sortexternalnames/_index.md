---
title: "SaveOptions.SortExternalNames"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SaveOptions özelliği. Dosya kaydedilmeden önce dış tanımlı adların sıralanıp sıralanmayacağını gösterir."
type: docs
url: /tr/net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir.

```csharp
public bool SortExternalNames { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // SaveOptions'dan miras alan bir OoxmlSaveOptions örneği oluşturun.
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // SortExternalNames özelliğinin varsayılan değerini gösterin.
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // SortExternalNames özelliğini true olarak ayarlayın.
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // Belirtilen kaydetme seçenekleriyle çalışma kitabını kaydedin
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
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

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


