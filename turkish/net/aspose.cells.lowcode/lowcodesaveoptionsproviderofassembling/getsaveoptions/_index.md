---
title: "LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfAssembling yöntemi. Şu anda bölünmüş parça için çıktı ayarlarını alacağı kaydetme seçeneklerini getirir"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions method

Mevcut bölünmüş parça için çıktı ayarlarını almak üzere kaydetme seçeneklerini alır.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].Value = "Sample Data for Split";

            try
            {
                // LowCodeSaveOptionsProviderOfAssembling örneği oluştur
                var provider = new LowCodeSaveOptionsProviderOfAssembling
                {
                    PathHeader = "Output/",
                    PathTail = ".xlsx",
                    UseSheetName = true,
                    SheetPrefix = "Sheet_",
                    SplitPartPrefix = "Part_",
                    SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
                };

                // Yapıcı erişilemediği için yansıma kullanarak bir SplitPartInfo örneği oluşturun
                var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);

                // SplitPartInfo parametresiyle GetSaveOptions'ı çağırın
                LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);

                Console.WriteLine("SaveOptions created successfully");
                Console.WriteLine($"Output format: {saveOptions.SaveFormat}");

                // Çalışma kitabını kaydedin (gerçek kullanımda bu, oluşturulan kaydetme seçeneklerini kullanır)
                workbook.Save("GetSaveOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in GetSaveOptions demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


