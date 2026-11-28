---
title: "Sınıf GridHtmlSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.GridHtmlSaveOptions sınıfı. HTML dosyasını kaydetmek için seçenekleri temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

HTML dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor)() | HTML dosyası kaydetme seçeneklerini oluşturur. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor_1)(GridSaveFormat) | HTM dosyası kaydetme seçeneklerini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory/) { get; set; } | Ekli dosyaların kaydedileceği dizin. Yalnızca HTML akışına kaydetme için. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix/) { get; set; } | HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca HTML akışına kaydetme için. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder/) { get; set; } | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır. (Inherited from [`GridSaveOptions`](../gridsaveoptions/).) |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata/) { get; set; } | Dosyayı kaydettikten sonra çalışma kitabını boş bırak. (Inherited from [`GridSaveOptions`](../gridsaveoptions/).) |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory/) { get; set; } | True ise ve dizin mevcut değilse, dosyayı kaydetmeden önce dizin otomatik olarak oluşturulur. (Inherited from [`GridSaveOptions`](../gridsaveoptions/).) |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname/) { get; set; } | HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding/) { get; set; } | Ayarlanmamışsa, Encoding.UTF8 varsayılan kodlama türü olarak kullanılır. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Tüm çalışma kitabının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea/) { get; set; } | Mevcut aktif Çalışma Sayfasının dışa aktarılan CellArea'sını alır veya ayarlar. Bu özelliği ayarlarsanız, mevcut aktif Çalışma Sayfasının yazdırma alanı göz ardı edilecektir. Dosya html olarak kaydedilirken yalnızca belirtilen alan dışa aktarılacaktır. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines/) { get; set; } | Kılavuz çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings/) { get; set; } | Dosya html olarak kaydedilirken başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Html dosyasını Excel'e aktarmak istiyorsanız, varsayılan değeri koruyun. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet/) { get; set; } | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64/) { get; set; } | Görüntülerin HTML, MHTML veya EPUB formatında Base64 olarak kaydedilip kaydedilmeyeceğini belirtir. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly/) { get; set; } | Yalnızca yazdırma alanının HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab/) { get; set; } | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments/) { get; set; } | Dosya html olarak kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink/) { get; set; } | sheet00x.htm, filelist.xml ve tabstrip.htm içinde tam yol bağlantısı kullanılıp kullanılmayacağını gösterir. Varsayılan değer false'tur. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas/) { get; set; } | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. (Inherited from [`GridSaveOptions`](../gridsaveoptions/).) |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle/) { get; set; } | HTML sayfasının başlığı. Yalnızca html akışına kaydederken. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell/) { get; set; } | Hücrede html etiketini ayrıştır, örneğin <br> gibi, hücre değeri olarak ya da html etiketi olarak, varsayılan true'tur. |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference/) { get; set; } | Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız, değeri true olarak ayarlayın. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache/) { get; set; } | Grafik önbellek verilerinin yenilenip yenilenmeyeceğini gösterir. (Inherited from [`GridSaveOptions`](../gridsaveoptions/).) |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat/) { get; } | Kaydedilen dosya formatını alır. (Inherited from [`GridSaveOptions`](../gridsaveoptions/).) |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames/) { get; set; } | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. (Inherited from [`GridSaveOptions`](../gridsaveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas/) { get; set; } | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. (Inherited from [`GridSaveOptions`](../gridsaveoptions/).) |

### Ayrıca Bakınız

* class [GridSaveOptions](../gridsaveoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


