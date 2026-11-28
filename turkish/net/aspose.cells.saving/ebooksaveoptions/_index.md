---
title: "Class EbookSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Saving.EbookSaveOptions class. e-kitap dosyasını kaydetme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

e-kitap dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | E-kitap dosyasını kaydetmek için seçenekler oluşturur. |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | E-kitap dosyasını kaydetmek için seçenekler oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | CSS font-family'ye genel bir yazı tipi eklenip eklenmeyeceğini gösterir. Varsayılan değer true(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Veri tam olarak gösterilemediğinde araç ipucu metni eklenip eklenmeyeceğini gösterir. Varsayılan değer false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Ekli dosyaların kaydedileceği dizin. Yalnızca html akışına kaydederken kullanılır.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Html dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca html akışına kaydederken kullanılır.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Html dosyasını kaydetmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | CSS adının önekini alır ve ayarlar, varsayılan değer ""'dır.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Yazılacak CellName'i gösteren özniteliği belirtir. (ör. Değer "id" ise, hücre "A1" için çıktı &lt;td id='A1'&gt; olur). Varsayılan değer null.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir metin değerine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dosya kaydedildikten sonra çalışma kitabını boşalt.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | True ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Biçimlendirici için ek CSS stillerini alır veya ayarlar. Yalnızca [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) True olduğunda çalışır. CssStyles="body { padding: 5px }";(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Excel dosyalarını html dosyalarına dönüştürürken DataBar'ın nasıl render edileceği modunu temsil eder. Varsayılan değer BackgroundColor'dir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Html dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Yalnızca satır içi stillerin uygulanıp uygulanmayacağını, CSS'ye dayanılmadan gösterir. Varsayılan değer false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Dosya html'ye dışa aktarılırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | HTML dosyasına gömülecek yazı tipi dosyasının türünü alır veya ayarlar. Varsayılan değer None'dir ve bu, HTML'e hiçbir yazı tipinin gömülmeyeceği anlamına gelir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | HTML çıktısını CSS özel özellikleri kullanarak optimize eder. Örneğin, aynı base64 görüntünün birden çok kez göründüğü senaryoda, özel özellik sayesinde görüntü verisi yalnızca bir kez kaydedilir, böylece ortaya çıkan HTML'in performansı artırılabilir. Varsayılan değer false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmediğini gösterir. (ör. "&amp;nbsp;" "&amp;#160;" ile değiştirilir). Varsayılan değer false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer true'dır.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Kullanılmayan stillerin dışlanıp dışlanmayacağını gösterir. Oluşturulan html dosyalarında, kullanılmayan stillerin dışlanması dosya boyutunu görsel etkilere zarar vermeden küçültebilir. Bu özelliğin varsayılan değeri true'dır. Kullanıcı, oluşturulan html için çalışma kitabındaki tüm stilleri (örneğin, daha sonra html'den çalışma kitabını geri yükleme senaryosu gibi) tutması gerekiyorsa, lütfen bu özelliği false olarak ayarlayın.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Yalnızca aktif çalışma sayfasının html dosyasına aktarılıp aktarılmayacağını gösterir. True ise sadece aktif çalışma sayfası html dosyasına aktarılır; False ise tüm çalışma kitabı html dosyasına aktarılır. Varsayılan değer false'tur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Mevcut aktif Çalışma Sayfasının dışa aktarılacak CellArea'ını alır veya ayarlar. Bu özelliği ayarlarsanız, mevcut aktif Çalışma Sayfasının yazdırma alanı atlanır. Dosya html olarak kaydedilirken yalnızca belirtilen alan dışa aktarılır.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Sahte alt satır verisinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. Html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Dosya html olarak kaydedilirken boş olmayan hücrelerin excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Çıktı html'yi excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Yorumların html dosyalarına dışa aktarım tipini temsil eder.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Html dosyası verisinin dışa aktarım kuralını gösterir. Varsayılan değer All'dir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dır. Html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Metin uzunluğu maksimum görüntüleme sütunundan uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Html dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Dosya html olarak kaydedilirken formüllerin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dır. Çıktı html'yi excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Çerçeve betiklerinin ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dır. Html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Kılavuz çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dır.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Görsellerin HTML, MHTML veya EPUB formatında Base64 olarak kaydedilip kaydedilmeyeceğini belirtir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | HTML olarak kaydederken adlandırılmış aralıklar için bağlantı (anchor) öğelerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Eski.**) Nesneleri dışa aktarmak için ExportObjectListener'ı alır veya ayarlar.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Yalnızca yazdırma alanının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'dur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Tarayıcılar tarafından desteklenmeyen kenarlık stilinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını gösterir. html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. Varsayılan değer false'dur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'dur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Çalışma sayfası CSS'inin ayrı ayrı dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'dur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Çalışma sayfasını ayrı ayrı html'ye dışa aktarmak için IFilePathProvider'ı alır veya ayarlar.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Sütunu taşan hücrenin tüm biçimlendirilmiş verisinin gösterilip gösterilmeyeceğini belirtir. true ise sütun genişliği göz ardı edilir ve hücrenin tüm verisi dışa aktarılır. false ise veri Excel gibi dışa aktarılır. Varsayılan değer false'dur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Excel'de gizli sütun (bu sütunun genişliği 0) html formatına kaydedilmeden önce, HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya eklenmez, değer "Hidden" ise sütun çıktıya eklenir ancak gizli olur, varsayılan değer "Hidden"dır.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Excel'de gizli satır (bu satırın yüksekliği 0) html formatına kaydedilmeden önce, HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya eklenmez, değer "Hidden" ise satır çıktıya eklenir ancak gizli olur, varsayılan değer "Hidden"dır.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Hücre formatı satır içi kaydırma (wrap text) olarak ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. Varsayılan değer false'tur(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Excel dosyasını html formatında kaydederken hücreler arası bir dizeyin MS Excel ile aynı şekilde görüntülenip görüntülenmeyeceğini gösterir. Varsayılan değer Default'tır, bu yüzden hücreler arası dizeler için Aspose.Cells ve MS Excel tarafından oluşturulan html dosyaları arasında çok az fark vardır. Ancak büyük html dosyaları oluşturma performansı açısından, değeri Cross olarak ayarlamak, Default veya Fit2Cell'e göre birkaç kat daha hızlı olur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | HTML formatını kaydederken kullanılacak HTML standardı sürümünü belirtir. Varsayılan değer HtmlVersion.Default'tir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Görünür olmayan şekillerin dışa aktarılıp aktarılmayacağını belirtir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Dışa aktarmadan önce ImageOrPrintOptions nesnesini alın.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Görüntü genişliğini ölçeklenebilir birimle tanımlarken sütun genişliğini ölçeklenebilir birimle tanımlama durumunu gösterir. Varsayılan değer true'dur. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Tablo kenarlıklarının çöküp çökmediğini gösterir. Varsayılan değer true'dur. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Görüntü dosyalarının geçici dizine aktarılıp aktarılmadığını gösterir. Yalnızca HTML akışına kaydederken geçerlidir. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Dosya HTML olarak kaydedilirken yorumların dışa aktarılıp aktarılmadığını gösterir, varsayılan değer false'tur. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | sheet00x.htm, filelist.xml ve tabstrip.htm içinde tam yol bağlantısı kullanılıp kullanılmadığını gösterir. Varsayılan değer false'tur. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | JavaScript'in JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. Varsayılan değer true'dur. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | HTML'ye kaydederken düzen modunu alır veya ayarlar. Varsayılan değer Normal'dir (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | `<a>` bağlantısındaki target özniteliğinin tipini gösterir. Varsayılan değer HtmlLinkTargetType.Parent'dir. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. (Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Dosya HTML'ye dışa aktarılırken boş TD öğesinin zorunlu birleştirilip birleştirilmeyeceğini gösterir. Değer true olarak ayarlandığında HTML dosyasının boyutu önemli ölçüde azalacaktır. Varsayılan değer false'tur. HTML dosyasını Excel'e içe aktarmak veya dosyayı HTML olarak kaydederken mükemmel ızgara çizgileri dışa aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Ardışık boş hücreleri (boş td öğeleri) birleştirme seçeneği. Varsayılan değer MergeEmptyTdType.Default'dir. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | OfficeMath nesnelerinin HTML'ye nasıl dışa aktarıldığını gösterir, varsayılan değer Image'dir. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | HTML sayfasının başlığı. Yalnızca HTML akışına kaydederken kullanılır. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Hücredeki HTML etiketi (örneğin `<div></div>`) hücre değeri olarak ayrıştırılmalı mı yoksa olduğu gibi korunmalı mı olduğunu gösterir. Varsayılan değer true'dur. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | HTML veya MHT dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız, değeri true olarak ayarlayın. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. (Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | HTML'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan değer false'tur. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Kaydedilen dosya formatını alır. (Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Tek bir HTML dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini gösterir. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | HTML çıktısında boşlukların nasıl işlendiğini gösterir. Bu seçenek şu anda yalnızca sayısal biçimlere (ör. muhasebe biçimi) uygulanır. Varsayılan değer Css'dir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | tr, col, td gibi tip css adının önekini alır ve ayarlar, bu önek belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. Varsayılan değer ""'dir.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'dur.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Uyarı geri çağrısını alır veya ayarlar.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Sütun genişliğinin ölçek biriminde html'ye aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'dur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Dosya html'ye kaydedilirken çalışma sayfası yakınlaştırma seviyesi üzerinden html'yi yakınlaştırıp uzaklaştırıp uzaklaştırmayacağını gösterir, varsayılan değer false'dur.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // EbookSaveOptions sınıfının bir örneğini oluşturun
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // Özellikleri ayarlama
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // Çalışma kitabını belirtilen seçeneklerle bir HTML dosyasına kaydedin
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


