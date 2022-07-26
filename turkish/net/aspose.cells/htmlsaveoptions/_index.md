---
title: HtmlSaveOptions
second_title: Aspose.Cells for .NET API Referansı
description: Html dosyasını kaydetme seçeneklerini temsil eder.
type: docs
weight: 3740
url: /tr/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Html dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | Html dosyasını kaydetmek için seçenekler oluşturur. |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | htm dosyasını kaydetmek için seçenekler oluşturur. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | Veriler tam olarak görüntülenemediğinde araç ipucu metninin eklenip eklenmeyeceğini belirtir. Varsayılan değer false'tur. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | Eklenen dosyaların kaydedileceği dizin. Yalnızca html akışına kaydetmek için. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | html dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca html akışına kaydetmek için. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | css adının önekini alır ve ayarlar, varsayılan değer ""'dir. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Dosyayı kaydettikten sonra çalışma kitabını boşaltın. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Doğruysa ve dizin yoksa, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | Html'yi dışa aktarmak için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut olmadığında varsayılan yazı tipi kullanılacaktır, Bu özellik boşsa, Aspose.Cells orijinal yazı tipi ile aynı aileye sahip evrensel yazı tipini kullanır, varsayılan değer null. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | Dosyayı html'ye aktarırken Alt Düzeyde açıklanan koşullu yorumların devre dışı bırakılıp bırakılmadığını gösterir, varsayılan değer false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | Ayarlanmadıysa, varsayılan kodlama türü olarak Encoding.UTF8'i kullanın. |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | Kullanılmayan stilleri hariç tutup tutmadığını gösterme. Oluşturulan html dosyaları için, kullanılmayan stilleri hariç tutmak, görsel efektleri etkilemeden dosya boyutunu küçültebilir. Bu nedenle, bu özelliğin varsayılan değeri true'dur. Kullanıcının oluşturulan html için çalışma kitabındaki tüm stilleri tutması gerekiyorsa (kullanıcı 'nin çalışma kitabını daha sonra oluşturulan html'den geri yüklemesi gerektiği senaryosu gibi), lütfen bu özelliği false olarak ayarlayın. . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | Tüm çalışma kitabının html dosyasına aktarılıp aktarılmadığını gösterir. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | Geçerli etkin Çalışma Sayfasının dışa aktarılan Hücre Alanı'nı alır veya ayarlar. Bu özniteliği ayarlarsanız, geçerli etkin Çalışma Sayfasının yazdırma alanı atlanır. Dosya html'ye kaydedilirken yalnızca belirtilen alan dışa aktarılır. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | Sahte alt satır verilerinin dışa aktarılıp aktarılmadığını gösterir. Varsayılan değer true'dur. Eğer html veya mht file dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | Dosyayı html'ye kaydederken boş olmayan hücrelerin excel koordinatının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'dir. Çıktı html'yi excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | Html dosya verilerini dışa aktarma kuralını belirtir.Varsayılan değer All'dır. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | Belge özelliklerinin dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer doğrudur. html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | Metnin uzunluğu maksimum görüntüleme sütunundan uzun olduğunda fazladan başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer yanlıştır. Html dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | Dosyayı html'ye kaydederken formülün dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. Çıktı html'yi excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | Çerçeve komut dosyalarının ve belge özelliklerinin dışa aktarılıp aktarılmayacağını belirtir. Varsayılan değer true'dur. Eğer html veya mht file dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | Kılavuz çizgilerinin dışa aktarılıp dışa aktarılmadığını gösterir. Varsayılan değer yanlıştır. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmadığını gösterir.Varsayılan değer doğrudur. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | Görüntülerin Base64 biçiminde HTML, MHTML veya EPUB'a kaydedilip kaydedilmeyeceğini belirtir. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını belirtir. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını belirtir. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | Yalnızca yazdırma alanının html dosyasına aktarılıp aktarılmadığını gösterir. Varsayılan değer false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | Kenarlık stili tarayıcılar tarafından desteklenmediğinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını belirtir. html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. Varsayılan değer false'dir. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer doğrudur. html veya mht dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | Çalışma sayfası css'inin ayrı olarak dışa aktarılıp aktarılmayacağını belirtir. Varsayılan değer false'tur. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmadığını gösterir. Varsayılan değer doğrudur. html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | Çalışma Sayfasını html'ye ayrı olarak dışa aktarmak için IFilePathProvider'ı alır veya ayarlar. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | Excel'de Gizli sütun (bu sütunun genişliği 0), bunu html biçiminde kaydetmeden önce, HtmlHiddenColDisplayType "Kaldır" ise, gizli sütun çıkmaz, değer "Gizli" ise, sütun çıktı, ancak gizlendi, varsayılan değer "Gizli" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | Excel'de Gizli satır(bu satırın yüksekliği 0'dır), bunu html biçiminde kaydetmeden önce, HtmlHiddenRowDisplayType "Kaldır" ise, gizli satır çıkmaz, değer "Gizli" ise, satır çıktı, ancak gizlendi, varsayılan değer "Gizli" |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | Bir Excel dosyasını html biçiminde kaydederken bir hücreler arası dizenin MS Excel ile aynı şekilde görüntülenip görüntülenmeyeceğini belirtir. Varsayılan olarak değer Varsayılan'dır, bu nedenle, hücreler arası dizeler için html arasında çok az fark vardır. Aspose.Cells ve MS Excel tarafından oluşturulan dosyalar. Ancak büyük html dosyaları oluşturma performansı, değeri Cross olarak ayarlamak, Default veya Fit2Cell. olarak ayarlamaktan birkaç kat daha hızlı olacaktır. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | Görünmeyen şekillerin dışa aktarılıp aktarılmayacağını belirtin |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | Dışa aktarmadan önce ImageOrPrintOptions nesnesini alın |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | Sütun genişliğini açıklamak için ölçeklenebilir birim kullanılırken, görüntü width 'yi açıklamak için ölçeklenebilir birim kullanılıp kullanılmayacağını belirtir. Varsayılan değer true'dur. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | Görüntü dosyalarının geçici dizine aktarılıp aktarılmayacağını belirtir. Yalnızca html akışına kaydetmek için. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | Dosya html'ye kaydedilirken yorumlar dışa aktarılırsa, varsayılan değerin false olduğunu gösterir. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | Sheet00x.htm, filelist.xml ve tabstrip.htm. 'de tam yol bağlantısının kullanılıp kullanılmadığını gösterme Varsayılan değer false. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | &lt;a&gt; bağlantısındaki hedef özniteliğin türünü belirtir,Varsayılan değer HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Dosyayı kaydetmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | Dosyayı html'ye aktarırken boş TD öğesinin zorla birleştirilip birleştirilmeyeceğini gösterir. Değer true olarak ayarlandıktan sonra html dosyasının boyutu önemli ölçüde azalacaktır. Varsayılan değer yanlıştır. html dosyasını excel'e aktarmak veya dosyayı html'ye kaydederken mükemmel ızgara çizgilerini dışa aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | Html sayfasının başlığı. Yalnızca html akışına kaydetmek içindir. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | Hücredeki html etiketini ayrıştır, beğen , hücre değeri olarak veya html etiketi olarak, varsayılan değer true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | html veya mht dosyasının sunum tercihi olduğunu belirtir. Varsayılan değer false'tur. daha güzel bir sunum elde etmek istiyorsanız, lütfen değeri true olarak ayarlayın. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Grafik önbelleği verilerinin yenilenip yenilenmediğini gösterir |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | Html'nin tek dosya olarak kaydedilip kaydedilmeyeceğini belirtir. Varsayılan değer false'dir. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Kayıt dosyası biçimini alır. |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | Tek bir html dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini belirtir. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Dosyayı kaydetmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Dosyayı kaydetmeden önce tanımlanmış adların sıralanıp sıralanmayacağını gösterir. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | tr,col,td ve benzeri gibi css türünün önekini alır ve ayarlar, bunlar belirli TableCssId özniteliğine sahip olan tablo öğesinde bulunur. Varsayılan değer "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Akıllı sanat ayarının güncellenip güncellenmediğini gösterir. Varsayılan değer false'tur. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Dosyayı kaydetmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Uyarı geri aramasını alır veya ayarlar. |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | Dosyayı html'ye aktarırken sütun genişliğini tanımlamak için ölçeklenebilir birimin kullanılıp kullanılmadığını gösterir. Varsayılan değer false'dir. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | Dosyayı html'ye kaydederken çalışma sayfası yakınlaştırma düzeyi aracılığıyla html'ye yakınlaştırma veya uzaklaştırma yapıldığını gösterir, varsayılan değer false. |

### Ayrıca bakınız

* class [SaveOptions](../saveoptions)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
