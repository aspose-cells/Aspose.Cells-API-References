---
title: "Sınıf ImageSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ImageSaveOptions sınıfı. Görüntü kaydetme seçeneklerini temsil eder. Gelişmiş kullanım için lütfen WorkbookRender veya SheetRender kullanın"
type: docs
url: /tr/net/aspose.cells/imagesaveoptions/
---
## ImageSaveOptions class

Görüntü kaydetme seçeneklerini temsil eder. Gelişmiş kullanım için lütfen [`WorkbookRender`](../../aspose.cells.rendering/workbookrender/) veya [`SheetRender`](../../aspose.cells.rendering/sheetrender/) kullanın.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/#constructor)() | Görüntü dosyasını kaydetmek için seçenekleri oluşturur. |
| [ImageSaveOptions](imagesaveoptions/#constructor_1)(SaveFormat) | Görüntü dosyasını kaydetmek için seçenekleri oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dosya kaydedildikten sonra çalışma kitabını boş bırak. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer doğrudur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ImageOrPrintOptions](../../aspose.cells/imagesaveoptions/imageorprintoptions/) { get; } | Ek görüntü oluşturma seçenekleri. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Kaydetme dosya formatını alır. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [StreamProvider](../../aspose.cells/imagesaveoptions/streamprovider/) { get; set; } | Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Uyarı geri aramasını alır veya ayarlar. ([`SaveOptions`](../saveoptions/) sınıfından devralınmıştır.) |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Export");

            // Hedef yolu ayarlayın
            string destPath = "output.png";

            // Görüntü kaydetme seçenekleri oluşturun
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            
            // Kaydetme seçeneklerini özelleştirin
            saveOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            saveOptions.ImageOrPrintOptions.OnlyArea = true;

            // Çalışma kitabını görüntü seçenekleriyle kaydedin
            workbook.Save(destPath, saveOptions);

            Console.WriteLine("Image saved successfully to: " + destPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


