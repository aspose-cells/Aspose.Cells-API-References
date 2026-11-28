---
title: "LowCodeSaveOptionsProviderOfAssembling.UseSheetName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfAssembling özelliği. Dosya yolunu sayfa indeksi yerine sayfa adıyla oluşturup oluşturmayacağını belirler. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/
---
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property

Dosya yolunun sayfa indeksi yerine sayfa adıyla oluşturulup oluşturulmayacağı. Varsayılan değer false'tur.

```csharp
public bool UseSheetName { get; set; }
```

### Açıklamalar

Sayfa adı asla otomatik olarak yeniden oluşturulmaz. Bu nedenle true olarak ayarlandığında, geçersiz dosya yolu veya adı oluşturabilecek özel bir sayfa adı olmadığından emin olun.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
    {
        public static void Run()
        {
            // Adlandırılmış çalışma sayfası ile yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "MonthlyReport";
            
            // Bölme gösterimi için örnek veri ekleyin
            for(int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
            }

            // Sağlayıcıyı oluşturun ve yapılandırın
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "split_files/",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet_",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // UseSheetName=false (varsayılan) gösterin
            Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);

            // Özelliği değiştirin ve yeni davranışı gösterin
            provider.UseSheetName = true;
            Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


