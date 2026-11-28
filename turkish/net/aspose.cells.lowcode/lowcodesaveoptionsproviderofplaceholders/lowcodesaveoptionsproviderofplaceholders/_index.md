---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfPlaceHolders yapıcı. Belirtilen şablonlara göre kaydetme seçenekleri sağlamak için bir örnek oluşturur"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

Belirtilen şablonlara göre kaydetme seçenekleri sağlamak için bir örnek oluşturur.

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pathTemplate | String | Sonuç dosya yolunun şablonu. |

### Açıklamalar

Dosya yolu şablonunda desteklenen yer tutucular: ${SheetIndex}: bölünmüş parçanın sayfa indeksine, ${SheetName}: bölünmüş parçanın sayfa adına, ${SplitPartIndex}: bölünmüş parçanın indeksine, ${SheetIndexPrefix}: [`SheetIndexPrefix`](../sheetindexprefix/) ile değiştirilecek, ${SheetNamePrefix}: [`SheetNamePrefix`](../sheetnameprefix/) ile değiştirilecek, ${SplitPartPrefix}: [`SplitPartPrefix`](../splitpartprefix/) ile değiştirilecek

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // #ctor metodunu String parametresiyle çağırın
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // Bazı özellikleri ayarlayın
                provider.SheetIndexOffset = 0;
                provider.SplitPartIndexOffset = 0;
                provider.SheetNamePrefix = "Sheet_";
                provider.SplitPartPrefix = "Part_";

                Console.WriteLine("LowCodeSaveOptionsProviderOfPlaceHolders created successfully with path template: " + pathTemplate);
                Console.WriteLine($"SheetNamePrefix: {provider.SheetNamePrefix}, SplitPartPrefix: {provider.SplitPartPrefix}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LowCodeSaveOptionsProviderOfPlaceHolders: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


