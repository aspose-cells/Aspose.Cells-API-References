---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfPlaceHolders özelliği. Bölüm parçası indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur; yani yalnızca bir bölüm parçası olduğunda bölüm parçası indeksi ve ilgili prefixSplitPartPrefix dosya yoluna eklenmez."
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property

Bölüm parçası indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir bölüm parçası olduğunda bölüm parçası indeksi ve ilgili prefix([`SplitPartPrefix`](../splitpartprefix/)) dosya yoluna eklenmez.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            // Birden fazla bölüme ayrılmayacak verilerle çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Single Part Demonstration";

            // Tek bir bölümle sonuçlanan yol şablonu ve bölme koşuluyla sağlayıcı oluştur
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
            {
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            // Özelliğin false durumunu (varsayılan) göster
            Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
            provider.BuildPathWithSplitPartAlways = false;
            
            // Bu, yalnızca bir bölüm mevcut olduğunda Result.xlsx dosyasını oluşturur
            Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
            ExecuteDummySave(workbook, "Result.xlsx");

            // Özelliği değiştir ve true durumunu göster
            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
            
            // Bu, tek bölümde bile Result_0.xlsx dosyasını oluşturur
            ExecuteDummySave(workbook, "Result_0.xlsx");
        }

        private static void ExecuteDummySave(Workbook workbook, string filename)
        {
            // Gerçek kullanımda, sağlayıcı tabanlı kaydetme işlemiyle değiştir
            Console.WriteLine($"Simulated save operation -> Filename: {filename}");
            workbook.Save(filename, SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


