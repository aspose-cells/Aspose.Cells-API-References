---
title: "Sınıf MarkdownSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.MarkdownSaveOptions sınıfı. Markdown için kaydetme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/
---
## MarkdownSaveOptions class

Markdown için kaydetme seçeneklerini temsil eder.

```csharp
public class MarkdownSaveOptions : SaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MarkdownSaveOptions](markdownsaveoptions/)() | Markdown belgesini kaydetmek için seçenekler oluşturur |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlignColumnPadding](../../aspose.cells/markdownsaveoptions/aligncolumnpadding/) { get; set; } | Oluşturulan Markdown tabloları için sütun hizalamasının etkin olup olmadığını gösterir. Etkinleştirildiğinde, sütunlar belirtilen karakterle (genellikle boşluk için ' ') hücre içeriği doldurularak hizalanır. Sütun hizalamasını devre dışı bırakmak için '\\0' olarak ayarlayın (varsayılan). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CalculateFormula](../../aspose.cells/markdownsaveoptions/calculateformula/) { get; set; } | Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dosya kaydedildikten sonra çalışma kitabını boş bırak. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [Encoding](../../aspose.cells/markdownsaveoptions/encoding/) { get; set; } | Varsayılan kodlamayı alır ve ayarlar. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer doğrudur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ExportHyperlinkAsReference](../../aspose.cells/markdownsaveoptions/exporthyperlinkasreference/) { get; set; } | Hipermetin bağlantısını satır içi biçim yerine referans tanımlarıyla dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [ExportImagesAsBase64](../../aspose.cells/markdownsaveoptions/exportimagesasbase64/) { get; set; } | Görsellerin Markdown'a Base64 biçiminde kaydedilip kaydedilmeyeceğini belirtir. Varsayılan değer true'dur. |
| [FormatStrategy](../../aspose.cells/markdownsaveoptions/formatstrategy/) { get; set; } | Hücre değerini dize olarak dışa aktarırken format stratejisini alır ve ayarlar. |
| [ImageOptions](../../aspose.cells/markdownsaveoptions/imageoptions/) { get; } | Dışa aktarmadan önce ImageOrPrintOptions nesnesini alın |
| [LightCellsDataProvider](../../aspose.cells/markdownsaveoptions/lightcellsdataprovider/) { get; set; } | Hafif modda çalışma kitabını kaydetmek için hücre verilerini sağlayan Veri sağlayıcı. |
| [LineSeparator](../../aspose.cells/markdownsaveoptions/lineseparator/) { get; set; } | Satır ayırıcıyı alır ve ayarlar. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [OfficeMathOutputType](../../aspose.cells/markdownsaveoptions/officemathoutputtype/) { get; set; } | OfficeMath nesnelerinin Markdown'a nasıl dışa aktarıldığını gösterir, varsayılan değer Görüntü'dür. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Kaydetme dosya formatını alır. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SheetSet](../../aspose.cells/markdownsaveoptions/sheetset/) { get; set; } | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [`Active`](../../aspose.cells.rendering/sheetset/active/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SplitTablesByBlankRow](../../aspose.cells/markdownsaveoptions/splittablesbyblankrow/) { get; set; } | Çalışma sayfasındaki boş satırların Markdown'a dışa aktarılırken tablo ayırıcıları olarak ele alınıp alınmayacağını gösterir. Varsayılan değer false'tur. |
| [StreamProvider](../../aspose.cells/markdownsaveoptions/streamprovider/) { get; set; } | Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar. `null` ise, dışa aktarılan nesneler çıktı dosyasıyla aynı dizine kaydedilir. |
| [TableHeaderType](../../aspose.cells/markdownsaveoptions/tableheadertype/) { get; set; } | Tablo başlığının nasıl ayarlandığını alır ve ayarlar. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Uyarı geri aramasını alır veya ayarlar. ([`SaveOptions`](../saveoptions/) sınıfından devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class MarkdownSaveOptionsDemo
    {
        public static void MarkdownSaveOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // MarkdownSaveOptions örneği oluştur
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = "\n",
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Çalışma kitabını bir Markdown dosyası olarak kaydet
            workbook.Save("MarkdownSaveOptionsExample.md", saveOptions);

            Console.WriteLine("Workbook saved as Markdown file successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


