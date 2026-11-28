---
title: "LowCodeSaveOptionsProviderOfPlaceHolders sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders sınıfı. Bölünmüş parçaları dosyalara kaydeden ve ortaya çıkan dosyanın yolunun yer tutucularla tanımlandığı kaydetme seçeneklerini sağlamak için bir uygulama."
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

Bölünmüş parçaları dosyalara kaydeden ve ortaya çıkan dosyanın yolunun yer tutucularla tanımlandığı kaydetme seçeneklerini sağlamak için uygulanmıştır.

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | Belirtilen şablonlara göre kaydetme seçenekleri sağlamak için bir örnek oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | Sayfa dizini veya adının dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa dizini ve adı ve ilgili önek([`SheetNamePrefix`](./sheetnameprefix/)) dosya yoluna eklenmez. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | Bölünmüş parça dizininin dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça dizini ve ilgili önek([`SplitPartPrefix`](./splitpartprefix/)) dosya yoluna eklenmez. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | Kaydetme seçenekleri örneği oluşturmak için [`GetSaveOptions`](./getsaveoptions/) içindeki şablon. |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | Dosya yolunda kullanılan sayfa indeksi ile gerçek değeri ([`SheetIndex`](../splitpartinfo/sheetindex/)) arasındaki fark. |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | Çalışma sayfası indeksinin öneki. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | Çalışma sayfası indeksinin öneki. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | Dosya yolunda kullanılan bölünmüş parça indeksi ile gerçek değeri ([`PartIndex`](../splitpartinfo/partindex/)) arasındaki fark. |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | Bölünmüş parça indeksinin öneki. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Mevcut bölünmüş parçayı işledikten sonra kaynakları serbest bırakır. ([`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/) tarafından miras alınmıştır.) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | Mevcut bölünmüş parça için çıktı ayarlarını almak üzere kaydetme seçeneklerini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını örnek verilerle doldurun
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Yer tutucular içeren yol şablonu ile sağlayıcı oluştur.
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // Sağlayıcı özelliklerini yapılandır.
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // Kaydetme seçenekleri şablonunu yapılandır.
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Bölünmüş renderleme için görüntü veya yazdırma seçeneklerini yapılandır.
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // Bölünmüş yapılandırma ile sayfa renderı oluştur.
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


