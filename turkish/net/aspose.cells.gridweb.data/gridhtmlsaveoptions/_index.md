---
title: GridHtmlSaveOptions
second_title: Aspose.Cells for .NET API Referansı
description: Html dosyasını kaydetme seçeneklerini temsil eder.
type: docs
weight: 250
url: /tr/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Html dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor)() | Html dosyasını kaydetmek için seçenekler oluşturur. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor_1)(GridSaveFormat) | htm dosyasını kaydetmek için seçenekler oluşturur. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory) { get; set; } | Eklenen dosyaların kaydedileceği dizin. Yalnızca html akışına kaydetmek için. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix) { get; set; } | html dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca html akışına kaydetmek için. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder) { get; set; } | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır. |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata) { get; set; } | Dosyayı kaydettikten sonra çalışma kitabını boşaltın. |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory) { get; set; } | Doğruysa ve dizin yoksa, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname) { get; set; } | Html'yi dışa aktarmak için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut olmadığında varsayılan yazı tipi kullanılacaktır, Bu özellik boşsa, Aspose.Cells orijinal yazı tipi ile aynı aileye sahip evrensel yazı tipini kullanır, varsayılan değer null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding) { get; set; } | Ayarlanmadıysa, varsayılan kodlama türü olarak Encoding.UTF8'i kullanın. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly) { get; set; } | Tüm çalışma kitabının html dosyasına aktarılıp aktarılmadığını gösterir. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea) { get; set; } | Geçerli etkin Çalışma Sayfasının dışa aktarılan Hücre Alanı'nı alır veya ayarlar. Bu özniteliği ayarlarsanız, geçerli etkin Çalışma Sayfasının yazdırma alanı atlanır. Dosya html'ye kaydedilirken yalnızca belirtilen alan dışa aktarılır. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines) { get; set; } | Kılavuz çizgilerinin dışa aktarılıp dışa aktarılmadığını gösterir. Varsayılan değer yanlıştır. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings) { get; set; } | Dosyayı html'ye kaydederken başlıkların dışa aktarılıp aktarılmayacağını gösterir.Varsayılan değer false'dir. Eğer html dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet) { get; set; } | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmadığını gösterir.Varsayılan değer doğrudur. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64) { get; set; } | Görüntülerin Base64 biçiminde HTML, MHTML veya EPUB'a kaydedilip kaydedilmeyeceğini belirtir. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly) { get; set; } | Yalnızca yazdırma alanının html dosyasına aktarılıp aktarılmadığını gösterir. Varsayılan değer false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab) { get; set; } | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments) { get; set; } | Dosya html'ye kaydedilirken yorumlar dışa aktarılırsa, varsayılan değerin false olduğunu gösterir. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink) { get; set; } | Sheet00x.htm, filelist.xml ve tabstrip.htm. 'de tam yol bağlantısının kullanılıp kullanılmadığını gösterme Varsayılan değer false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas) { get; set; } | Dosyayı kaydetmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle) { get; set; } | Html sayfasının başlığı. Yalnızca html akışına kaydetmek içindir. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell) { get; set; } | Hücredeki html etiketini ayrıştır, beğen , hücre değeri olarak veya html etiketi olarak, varsayılan değer true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference) { get; set; } | html veya mht dosyasının sunum tercihi olduğunu belirtir. Varsayılan değer false'tur. daha güzel bir sunum elde etmek istiyorsanız, lütfen değeri true olarak ayarlayın. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache) { get; set; } | Grafik önbelleği verilerinin yenilenip yenilenmediğini gösterir |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat) { get; } | Kayıt dosyası biçimini alır. |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames) { get; set; } | Dosyayı kaydetmeden önce tanımlanmış adların sıralanıp sıralanmayacağını gösterir. |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas) { get; set; } | Dosyayı kaydetmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |

### Ayrıca bakınız

* class [GridSaveOptions](../gridsaveoptions)
* ad alanı [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* toplantı [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
