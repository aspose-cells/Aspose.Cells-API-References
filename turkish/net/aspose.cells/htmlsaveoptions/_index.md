---
title: "Sınıf HtmlSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlSaveOptions sınıfı. HTML dosyası kaydetme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

HTML dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | HTML dosyası kaydetme seçeneklerini oluşturur. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | HTM dosyası kaydetme seçeneklerini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | CSS font-family'ye genel bir yazı tipinin eklenip eklenmeyeceğini gösterir. Varsayılan değer true'tur. |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Veri tam olarak görüntülenemediğinde araç ipucu metni eklenip eklenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Ekli dosyaların kaydedileceği dizin. Yalnızca HTML akışına kaydetme için. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca HTML akışına kaydetme için. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | CSS adının önekini alır ve ayarlar, varsayılan değer "". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Yazılacak CellName'i belirten özniteliği belirtir. (ör. Değer "id" ise, "A1" hücresi için çıktı &lt;td id='A1'&gt; olur). Varsayılan değer null'dur. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dosya kaydedildikten sonra çalışma kitabını boş bırak. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Biçimlendirici için ek CSS stillerini alır veya ayarlar. Yalnızca [`SaveAsSingleFile`](./saveassinglefile/) True olduğunda çalışır. CssStyles="body { padding: 5px }"; |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Excel dosyalarını HTML dosyalarına dönüştürürken DataBar'ın nasıl render edileceği modunu temsil eder. Varsayılan değer BackgroundColor. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Yalnızca satır içi stillerin uygulanıp uygulanmayacağını, CSS'ye dayanılmadan gösterir. Varsayılan değer false'tur. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Dosya HTML'ye dışa aktarılırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false'tur. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Yazı tipi dosyasının HTML dosyasına gömülme türünü alır veya ayarlar. Varsayılan değer None'dır ve bu, HTML'ye yazı tipi gömülmeyeceği anlamına gelir. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | HTML çıktısını CSS özel özellikleri kullanarak optimize eder. Örneğin, bir base64 görüntünün birden çok kez kullanıldığı senaryoda, özel özellik sayesinde görüntü verisi sadece bir kez kaydedilir ve ortaya çıkan HTML'nin performansı artırılabilir. Varsayılan değer false'tur. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmediğini gösterir. (ör. "&amp;nbsp;" "&amp;#160;" ile değiştirilir). Varsayılan değer false'tur. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Ayarlanmamışsa, Encoding.UTF8 varsayılan kodlama türü olarak kullanılır. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer doğrudur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Kullanılmayan stillerin dışarıda bırakılıp bırakılmadığını gösterir. Oluşturulan HTML dosyalarında kullanılmayan stillerin dışarıda bırakılması, görsel etkilere zarar vermeden dosya boyutunu küçültebilir. Bu nedenle bu özelliğin varsayılan değeri true'tır. Kullanıcı, oluşturulan HTML'den (örneğin, daha sonra HTML'den çalışma kitabını geri yüklemek gerektiğinde) çalışma kitabındaki tüm stilleri korumak istiyorsa, lütfen bu özelliği false olarak ayarlayın. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Yalnızca aktif çalışma sayfasının HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. True ise sadece aktif çalışma sayfası dışa aktarılır; False ise tüm çalışma kitabı dışa aktarılır. Varsayılan değer false'tur. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Mevcut aktif Çalışma Sayfasının dışa aktarılacak CellArea'ını alır veya ayarlar. Bu özniteliği ayarlarsanız, mevcut aktif Çalışma Sayfasının yazdırma alanı atlanır. Dosya HTML'ye kaydedilirken yalnızca belirtilen alan dışa aktarılır. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Alt satırdaki sahte verilerin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Dosya HTML olarak kaydedilirken boş olmayan hücrelerin Excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Çıktı HTML'yi Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Yorumların HTML dosyalarına dışa aktarım türünü temsil eder. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | HTML dosya verilerinin dışa aktarım kuralını gösterir. Varsayılan değer All'dir. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Metin uzunluğu maksimum görüntüleme sütunundan daha uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. HTML dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Dosya HTML olarak kaydedilirken formüllerin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. Çıktı HTML'yi Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Çerçeve betiklerinin ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Kılavuz çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Sayfanın satır ve sütun başlıklarının HTML dosyalarına kaydedilirken dışa aktarılıp aktarılmayacağını gösterir. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Görüntülerin HTML, MHTML veya EPUB formatında Base64 olarak kaydedilip kaydedilmeyeceğini belirtir. |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | HTML olarak kaydedilirken adlandırılmış aralıklar için bağlantı (anchor) öğelerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Nesnelerin dışa aktarımı için ExportObjectListener'ı alır veya ayarlar. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Yalnızca yazdırma alanının HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Sayfanın satır ve sütun başlıklarının HTML dosyalarına kaydedilirken dışa aktarılıp aktarılmayacağını gösterir. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Tarayıcılar tarafından desteklenmeyen kenarlık stilinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını gösterir. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. Varsayılan değer false'tur. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Çalışma sayfası CSS'inin ayrı ayrı dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Çalışma sayfasını ayrı ayrı HTML'ye dışa aktarmak için IFilePathProvider'ı alır veya ayarlar. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Sütunu taşan hücrenin tüm biçimlendirilmiş verisinin gösterilip gösterilmeyeceğini gösterir. True ise sütun genişliği göz ardı edilir ve hücrenin tüm verisi dışa aktarılır. False ise veri Excel gibi dışa aktarılır. Varsayılan değer false'tur. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Excel'de gizli sütun (bu sütunun genişliği 0'dır), HTML formatına kaydetmeden önce, HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya dahil edilmez, değer "Hidden" ise sütun çıktıya dahil edilir ancak gizli kalır, varsayılan değer "Hidden"'dır. |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Gizli satır (bu satırın yüksekliği 0) Excel'de, bunu html formatına kaydetmeden önce, HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya dahil edilmez, değer "Hidden" ise satır çıktıya dahil edilir ancak gizli kalır, varsayılan değer "Hidden"dır |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Hücre biçimi satır kaydırma olarak ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. Varsayılan değer false. |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Excel dosyasını html formatında kaydederken çapraz hücre dizesinin MS Excel ile aynı şekilde görüntülenip görüntülenmeyeceğini gösterir. Varsayılan değer "Default"'tır, bu nedenle çapraz hücre dizileri için Aspose.Cells ve MS Excel tarafından oluşturulan html dosyaları arasında çok az fark vardır. Ancak büyük html dosyaları oluştururken, değeri "Cross" olarak ayarlamak, "Default" veya "Fit2Cell"'e göre birkaç kat daha hızlı olur. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | HTML standardının hangi sürümünün HTML formatı kaydedilirken kullanılacağını belirtir. Varsayılan değer "HtmlVersion.Default"'tır. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Görünür olmayan şekillerin dışa aktarılıp aktarılmayacağını gösterir |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Dışa aktarmadan önce ImageOrPrintOptions nesnesini alın |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Sütun genişliğini tanımlamak için ölçeklenebilir birim kullanırken görüntü genişliğini ölçeklenebilir birimle tanımlayıp tanımlamayacağını gösterir. Varsayılan değer true'tur. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Tablo kenarlıklarının çökertilip çökertilmeyeceğini gösterir. Varsayılan değer true'tur. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Görüntü dosyalarının geçici dizine dışa aktarılıp aktarılmayacağını gösterir. Yalnızca html akışına kaydederken. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Dosya html olarak kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | sheet00x.htm, filelist.xml ve tabstrip.htm içinde tam yol bağlantısı kullanılıp kullanılmayacağını gösterir. Varsayılan değer false'tur. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur. |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | JavaScript'in JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. Varsayılan değer true'tur. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | HTML olarak kaydederken düzen modunu alır veya ayarlar. Varsayılan değer Normal'dir. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | `<a>` bağlantısındaki target özniteliğinin tipini gösterir. Varsayılan değer HtmlLinkTargetType.Parent'dır. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Boş TD öğesinin html'e dışa aktarılırken zorunlu birleştirilip birleştirilmeyeceğini gösterir. Değer true olarak ayarlandığında html dosyasının boyutu önemli ölçüde azalır. Varsayılan değer false'tur. Html dosyasını Excel'e içe aktarmak veya html olarak kaydederken mükemmel ızgara çizgileri dışa aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Ardışık boş hücreleri (boş td öğeleri) birleştirme seçeneği. Varsayılan değer MergeEmptyTdType.Default'tır. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | OfficeMath nesnelerinin HTML'ye nasıl dışa aktarılacağını gösterir, Varsayılan değer Image'dir. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | HTML sayfasının başlığı. Yalnızca html akışına kaydederken. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Hücredeki html etiketi (örneğin `<div></div>`) hücre değeri olarak ayrıştırılsın mı yoksa olduğu gibi korunsun mu olduğunu gösterir. Varsayılan değer true'tur. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız, değeri true olarak ayarlayın. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | HTML'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Kaydetme dosya formatını alır. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Render edilecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Tek bir html dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini gösterir. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | HTML çıktısında boşlukların nasıl işlendiğini gösterir. Bu seçenek şu anda yalnızca sayısal biçimlere (ör. muhasebe biçimi) uygulanmaktadır. Varsayılan değer Css. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Nesneleri dışa aktarmak için IStreamProvider'ı alır veya ayarlar. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | tr, col, td vb. gibi tip css adının önekini alır ve ayarlar; bu önek, belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. Varsayılan değer "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. ([`SaveOptions`](../saveoptions/) sınıfından kalıtılmıştır.) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Uyarı geri aramasını alır veya ayarlar. ([`SaveOptions`](../saveoptions/) sınıfından devralınmıştır.) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Sütun genişliğinin ölçek birimi olarak HTML'ye dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Dosya HTML olarak kaydedilirken çalışma sayfası yakınlaştırma düzeyiyle HTML'yi yakınlaştırıp uzaklaştırmayacağını gösterir, varsayılan değer false. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // HtmlSaveOptions bir örnek oluşturun
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = "",
                TableCssId = "",
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Çalışma kitabını HTML olarak kaydet
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


