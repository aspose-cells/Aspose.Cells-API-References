---
title: "Sınıf LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling sınıfı. Bölünmüş parçaları dosyalara kaydeden ve ortaya çıkan dosyanın yolunun PathHeaderSheetPrefixSheetIndexor SheetName SplitPartPrefixSplitPartIndexPathTail gibi dizinler içerebileceği şekilde adlandırılması için kaydetme seçeneklerini sağlayan bir uygulama."
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

Bölünmüş parçaları dosyalara kaydeden ve ortaya çıkan dosyanın yolunun (dizinler içerebilir) şu şekilde adlandırıldığı kaydetme seçeneklerini sağlamak için bir uygulama: [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(veya SheetName)+[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | Sayfa indeksinin veya adının dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa indeksi (veya adı) ve ilgili önek dosya yoluna eklenmez. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | Bölünmüş parça indeksinin dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir bölünmüş parça olduğunda, bölünmüş parça indeksi ve ilgili önek dosya yoluna eklenmez. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | Dosya yolunun başlık kısmı (sayfa ve bölünmüş parça içeriği eklenmeden önce). |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | Dosya yolunun son kısmı (sıra numaralarından sonra). Dosya adı uzantısını içermelidir. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | Kaydetme seçenekleri örneği oluşturmak için [`GetSaveOptions`](./getsaveoptions/) içindeki şablon. |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | Dosya yolunda kullanılan sayfa indeksi ile gerçek değeri ([`SheetIndex`](../splitpartinfo/sheetindex/)) arasındaki fark. |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | Çalışma sayfası indeksinin öneki. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | Dosya yolunda kullanılan bölünmüş parça indeksi ile gerçek değeri ([`PartIndex`](../splitpartinfo/partindex/)) arasındaki fark. |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | Bölünmüş parça indeksinin öneki. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | Dosya yolunun sayfa indeksi yerine sayfa adıyla oluşturulup oluşturulmayacağı. Varsayılan değer false'tur. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Mevcut bölünmüş parçayı işledikten sonra kaynakları serbest bırakır. ([`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/) tarafından miras alınmıştır.) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | Mevcut bölünmüş parça için çıktı ayarlarını almak üzere kaydetme seçeneklerini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // Kaydetme seçenekleri sağlayıcısını başlat ve yapılandır
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // LowCodeSaveOptions kullanarak bölme ile XLSX kaydetme seçeneklerini yapılandır
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Doğru kaydetme formatını kullanarak sağlayıcı etkin seçeneklerle çalışma kitabını kaydet
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


