---
title: "EbookSaveOptions Sınıfı"
linktitle: "EbookSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "EbookSaveOptions sınıfı. Go'da ebooksaveoptions'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/ebooksaveoptions/
---

## EbookSaveOptions class

e-kitap dosyasını kaydetme seçeneklerini temsil eder.

```go

type EbookSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewEbookSaveOptions](./newebooksaveoptions/) | E-kitap dosyasını kaydetmek için seçenekler oluşturur. |
| [NewEbookSaveOptions_SaveFormat](./newebooksaveoptions_saveformat/) | E-kitap dosyasını kaydetmek için seçenekler oluşturur. |
| [NewEbookSaveOptions_HtmlSaveOptions](./newebooksaveoptions_htmlsaveoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | Görünür olmayan şekillerin dışa aktarılıp aktarılmayacağını belirtir. |
| [SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | Görünür olmayan şekillerin dışa aktarılıp aktarılmayacağını belirtir. |
| [GetPageTitle](./getpagetitle/) | HTML sayfasının başlığı. Yalnızca HTML akışına kaydederken kullanılır. |
| [SetPageTitle](./setpagetitle/) | HTML sayfasının başlığı. Yalnızca HTML akışına kaydederken kullanılır. |
| [GetAttachedFilesDirectory](./getattachedfilesdirectory/) | Ekli dosyaların kaydedileceği dizin. Yalnızca HTML akışına kaydederken kullanılır. |
| [SetAttachedFilesDirectory](./setattachedfilesdirectory/) | Ekli dosyaların kaydedileceği dizin. Yalnızca HTML akışına kaydederken kullanılır. |
| [GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca HTML akışına kaydederken kullanılır. |
| [SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca HTML akışına kaydederken kullanılır. |
| [GetDefaultFontName](./getdefaultfontname/) | HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut olmadığında varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells orijinal yazı tipiyle aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur. |
| [SetDefaultFontName](./setdefaultfontname/) | HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut olmadığında varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells orijinal yazı tipiyle aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur. |
| [GetAddGenericFont](./getaddgenericfont/) | CSS font-family'ye genel bir yazı tipi eklenip eklenmeyeceğini gösterir. Varsayılan değer true'tur. |
| [SetAddGenericFont](./setaddgenericfont/) | CSS font-family'ye genel bir yazı tipi eklenip eklenmeyeceğini gösterir. Varsayılan değer true'tur. |
| [GetWorksheetScalable](./getworksheetscalable/) | html'i çalışma sayfası yakınlaştırma seviyesi üzerinden yakınlaştırma veya uzaklaştırma yaparken dosyayı html olarak kaydederken gösterir, varsayılan değer false'tur. |
| [SetWorksheetScalable](./setworksheetscalable/) | html'i çalışma sayfası yakınlaştırma seviyesi üzerinden yakınlaştırma veya uzaklaştırma yaparken dosyayı html olarak kaydederken gösterir, varsayılan değer false'tur. |
| [IsExportComments](./isexportcomments/) | Dosyayı html olarak kaydederken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur. |
| [SetIsExportComments](./setisexportcomments/) | Dosyayı html olarak kaydederken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur. |
| [GetExportCommentsType](./getexportcommentstype/) | Yorumların html dosyalarına dışa aktarım türünü temsil eder. |
| [SetExportCommentsType](./setexportcommentstype/) | Yorumların html dosyalarına dışa aktarım türünü temsil eder. |
| [GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | Dosyayı html olarak dışa aktarırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false'tur. |
| [SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | Dosyayı html olarak dışa aktarırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false'tur. |
| [IsExpImageToTempDir](./isexpimagetotempdir/) | Görüntü dosyalarının geçici dizine dışa aktarılıp aktarılmayacağını gösterir. Yalnızca html akışına kaydetmek için geçerlidir. |
| [SetIsExpImageToTempDir](./setisexpimagetotempdir/) | Görüntü dosyalarının geçici dizine dışa aktarılıp aktarılmayacağını gösterir. Yalnızca html akışına kaydetmek için geçerlidir. |
| [GetImageScalable](./getimagescalable/) | Görüntü genişliğini tanımlamak için ölçeklenebilir birim kullanılıp kullanılmayacağını, sütun genişliğini tanımlamak için ölçeklenebilir birim kullanıldığında gösterir. Varsayılan değer true'tur. |
| [SetImageScalable](./setimagescalable/) | Görüntü genişliğini tanımlamak için ölçeklenebilir birim kullanılıp kullanılmayacağını, sütun genişliğini tanımlamak için ölçeklenebilir birim kullanıldığında gösterir. Varsayılan değer true'tur. |
| [GetWidthScalable](./getwidthscalable/) | Sütun genişliğinin ölçek biriminde html'e dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetWidthScalable](./setwidthscalable/) | Sütun genişliğinin ölçek biriminde html'e dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [GetExportSingleTab](./getexportsingletab/) | Dosyanın yalnızca bir çalışma sayfası içerdiğinde tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetExportSingleTab](./setexportsingletab/) | Dosyanın yalnızca bir çalışma sayfası içerdiğinde tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Görüntülerin HTML, MHTML veya EPUB formatında Base64 olarak kaydedilip kaydedilmeyeceğini belirtir. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Görüntülerin HTML, MHTML veya EPUB formatında Base64 olarak kaydedilip kaydedilmeyeceğini belirtir. |
| [GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | Yalnızca etkin çalışma sayfasının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. True ise yalnızca etkin çalışma sayfası html dosyasına dışa aktarılır; false ise tüm çalışma kitabı html dosyasına dışa aktarılır. Varsayılan değer false'tur. |
| [SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | Yalnızca etkin çalışma sayfasının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. True ise yalnızca etkin çalışma sayfası html dosyasına dışa aktarılır; false ise tüm çalışma kitabı html dosyasına dışa aktarılır. Varsayılan değer false'tur. |
| [GetExportPrintAreaOnly](./getexportprintareaonly/) | Yalnızca yazdırma alanının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetExportPrintAreaOnly](./setexportprintareaonly/) | Yalnızca yazdırma alanının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [GetExportArea](./getexportarea/) | Mevcut etkin Worksheet'in dışa aktarılan CellArea'ını alır veya ayarlar. Bu özelliği ayarlarsanız, mevcut etkin Worksheet'in yazdırma alanı atlanır. Dosya html olarak kaydedilirken yalnızca belirtilen alan dışa aktarılır. |
| [SetExportArea](./setexportarea/) | Mevcut etkin Worksheet'in dışa aktarılan CellArea'ını alır veya ayarlar. Bu özelliği ayarlarsanız, mevcut etkin Worksheet'in yazdırma alanı atlanır. Dosya html olarak kaydedilirken yalnızca belirtilen alan dışa aktarılır. |
| [GetParseHtmlTagInCell](./getparsehtmltagincell/) | Hücredeki html etiketlerinin (örneğin <c>&lt;div&gt;&lt;/div&gt;</c>) hücre değeri olarak ayrıştırılıp ayrıştırılmayacağını veya olduğu gibi korunup korunmayacağını gösterir. Varsayılan değer true'tur. |
| [SetParseHtmlTagInCell](./setparsehtmltagincell/) | Hücredeki html etiketlerinin (örneğin <c>&lt;div&gt;&lt;/div&gt;</c>) hücre değeri olarak ayrıştırılıp ayrıştırılmayacağını veya olduğu gibi korunup korunmayacağını gösterir. Varsayılan değer true'tur. |
| [GetHtmlCrossStringType](./gethtmlcrossstringtype/) | Excel dosyasını html formatında kaydederken çapraz hücre dizesinin MS Excel'de olduğu gibi görüntülenip görüntülenmeyeceğini gösterir. Varsayılan değer Default'tır, bu nedenle çapraz hücre dizeleri için Aspose.Cells tarafından oluşturulan html dosyaları ile MS Excel arasında çok az fark vardır. Ancak büyük html dosyaları oluştururken değeri Cross olarak ayarlamak, Default veya Fit2Cell'e göre birkaç kat daha hızlı olur. |
| [SetHtmlCrossStringType](./sethtmlcrossstringtype/) | Excel dosyasını html formatında kaydederken çapraz hücre dizesinin MS Excel'de olduğu gibi görüntülenip görüntülenmeyeceğini gösterir. Varsayılan değer Default'tır, bu nedenle çapraz hücre dizeleri için Aspose.Cells tarafından oluşturulan html dosyaları ile MS Excel arasında çok az fark vardır. Ancak büyük html dosyaları oluştururken değeri Cross olarak ayarlamak, Default veya Fit2Cell'e göre birkaç kat daha hızlı olur. |
| [GetHiddenColDisplayType](./gethiddencoldisplaytype/) | Excel'de gizli sütun (bu sütunun genişliği 0) html formatına kaydedilmeden önce, HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya dahil edilmez, değer "Hidden" ise sütun çıktıya dahil edilir ancak gizli olarak kalır; varsayılan değer "Hidden"tır. |
| [SetHiddenColDisplayType](./sethiddencoldisplaytype/) | Excel'de gizli sütun (bu sütunun genişliği 0) html formatına kaydedilmeden önce, HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya dahil edilmez, değer "Hidden" ise sütun çıktıya dahil edilir ancak gizli olarak kalır; varsayılan değer "Hidden"tır. |
| [GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | Excel'de gizli satır (bu satırın yüksekliği 0) html formatına kaydedilmeden önce, HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya dahil edilmez, değer "Hidden" ise satır çıktıya dahil edilir ancak gizli olarak kalır; varsayılan değer "Hidden"tır. |
| [SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | Excel'de gizli satır (bu satırın yüksekliği 0) html formatına kaydedilmeden önce, HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya dahil edilmez, değer "Hidden" ise satır çıktıya dahil edilir ancak gizli olarak kalır; varsayılan değer "Hidden"tır. |
| [GetEncoding](./getencoding/) | Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır. |
| [SetEncoding](./setencoding/) | Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır. |
| [GetImageOptions](./getimageoptions/) | Dışa aktarmadan önce ImageOrPrintOptions nesnesini alın. |
| [GetSaveAsSingleFile](./getsaveassinglefile/) | Html'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetSaveAsSingleFile](./setsaveassinglefile/) | Html'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetShowAllSheets](./getshowallsheets/) | Tek bir html dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini gösterir. |
| [SetShowAllSheets](./setshowallsheets/) | Tek bir html dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini gösterir. |
| [GetExportPageHeaders](./getexportpageheaders/) | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [SetExportPageHeaders](./setexportpageheaders/) | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [GetExportPageFooters](./getexportpagefooters/) | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [SetExportPageFooters](./setexportpagefooters/) | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [GetExportHiddenWorksheet](./getexporthiddenworksheet/) | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. |
| [SetExportHiddenWorksheet](./setexporthiddenworksheet/) | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. |
| [GetPresentationPreference](./getpresentationpreference/) | Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız, değeri true olarak ayarlayın. |
| [SetPresentationPreference](./setpresentationpreference/) | Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız, değeri true olarak ayarlayın. |
| [GetCellCssPrefix](./getcellcssprefix/) | css adının önekini alır ve ayarlar, varsayılan değer "". |
| [SetCellCssPrefix](./setcellcssprefix/) | css adının önekini alır ve ayarlar, varsayılan değer "". |
| [GetTableCssId](./gettablecssid/) | tr, col, td vb. gibi tip css adının önekini alır ve ayarlar; bu önek, belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. Varsayılan değer "". |
| [SetTableCssId](./settablecssid/) | tr, col, td vb. gibi tip css adının önekini alır ve ayarlar; bu önek, belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. Varsayılan değer "". |
| [IsFullPathLink](./isfullpathlink/) | sheet00x.htm, filelist.xml ve tabstrip.htm içinde tam yol bağlantısı kullanılıp kullanılmadığını gösterir. Varsayılan değer false'tur. |
| [SetIsFullPathLink](./setisfullpathlink/) | sheet00x.htm, filelist.xml ve tabstrip.htm içinde tam yol bağlantısı kullanılıp kullanılmadığını gösterir. Varsayılan değer false'tur. |
| [GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | Çalışma sayfası CSS'sinin ayrı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | Çalışma sayfası CSS'sinin ayrı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | Tarayıcılar tarafından desteklenmeyen kenarlık stilinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını gösterir. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. Varsayılan değer false'tur. |
| [SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | Tarayıcılar tarafından desteklenmeyen kenarlık stilinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını gösterir. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. Varsayılan değer false'tur. |
| [GetMergeEmptyTdType](./getmergeemptytdtype/) | Ardışık boş hücreleri (boş td öğeleri) birleştirme seçeneği. Varsayılan değer MergeEmptyTdType.Default. |
| [SetMergeEmptyTdType](./setmergeemptytdtype/) | Ardışık boş hücreleri (boş td öğeleri) birleştirme seçeneği. Varsayılan değer MergeEmptyTdType.Default. |
| [GetExportCellCoordinate](./getexportcellcoordinate/) | Dosya HTML olarak kaydedilirken boş olmayan hücrelerin Excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Çıktı HTML'yi Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [SetExportCellCoordinate](./setexportcellcoordinate/) | Dosya HTML olarak kaydedilirken boş olmayan hücrelerin Excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Çıktı HTML'yi Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [GetExportExtraHeadings](./getexportextraheadings/) | Metin uzunluğu maksimum görüntüleme sütunundan uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. HTML dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [SetExportExtraHeadings](./setexportextraheadings/) | Metin uzunluğu maksimum görüntüleme sütunundan uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. HTML dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | HTML dosyalarına kaydedilirken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | HTML dosyalarına kaydedilirken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [GetExportFormula](./getexportformula/) | Dosya HTML olarak kaydedilirken formüllerin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. Çıktı HTML'yi Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [SetExportFormula](./setexportformula/) | Dosya HTML olarak kaydedilirken formüllerin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. Çıktı HTML'yi Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [GetAddTooltipText](./getaddtooltiptext/) | Veri tam olarak görüntülenemediğinde araç ipucu metninin eklenip eklenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetAddTooltipText](./setaddtooltiptext/) | Veri tam olarak görüntülenemediğinde araç ipucu metninin eklenip eklenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetExportGridLines](./getexportgridlines/) | Kılavuz çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetExportGridLines](./setexportgridlines/) | Kılavuz çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [GetExportBogusRowData](./getexportbogusrowdata/) | Sahte alt satır verilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [SetExportBogusRowData](./setexportbogusrowdata/) | Sahte alt satır verilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [GetExcludeUnusedStyles](./getexcludeunusedstyles/) | Kullanılmayan stillerin dışlanıp dışlanmayacağını gösterir. Oluşturulan HTML dosyalarında, kullanılmayan stillerin dışlanması dosya boyutunu görsel etkilere zarar vermeden küçültebilir. Bu nedenle bu özelliğin varsayılan değeri true'dur. Kullanıcı, oluşturulan HTML'de (örneğin, daha sonra HTML'den çalışma kitabını geri yükleme senaryosu gibi) çalışma kitabındaki tüm stilleri tutması gerekiyorsa, lütfen bu özelliği false olarak ayarlasın. |
| [SetExcludeUnusedStyles](./setexcludeunusedstyles/) | Kullanılmayan stillerin dışlanıp dışlanmayacağını gösterir. Oluşturulan HTML dosyalarında, kullanılmayan stillerin dışlanması dosya boyutunu görsel etkilere zarar vermeden küçültebilir. Bu nedenle bu özelliğin varsayılan değeri true'dur. Kullanıcı, oluşturulan HTML'de (örneğin, daha sonra HTML'den çalışma kitabını geri yükleme senaryosu gibi) çalışma kitabındaki tüm stilleri tutması gerekiyorsa, lütfen bu özelliği false olarak ayarlasın. |
| [GetExportDocumentProperties](./getexportdocumentproperties/) | Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [SetExportDocumentProperties](./setexportdocumentproperties/) | Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [GetExportWorksheetProperties](./getexportworksheetproperties/) | Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [SetExportWorksheetProperties](./setexportworksheetproperties/) | Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [GetExportWorkbookProperties](./getexportworkbookproperties/) | Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [SetExportWorkbookProperties](./setexportworkbookproperties/) | Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | Çerçeve betikleri ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | Çerçeve betikleri ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [GetExportDataOptions](./getexportdataoptions/) | HTML dosyası verilerinin dışa aktarım kuralını gösterir. Varsayılan değer All'dir. |
| [SetExportDataOptions](./setexportdataoptions/) | HTML dosyası verilerinin dışa aktarım kuralını gösterir. Varsayılan değer All'dir. |
| [GetLinkTargetType](./getlinktargettype/) | <c>&lt;a&gt;</c> bağlantısındaki target özniteliğinin tipini gösterir. Varsayılan değer HtmlLinkTargetType.Parent'dir. |
| [SetLinkTargetType](./setlinktargettype/) | <c>&lt;a&gt;</c> bağlantısındaki target özniteliğinin tipini gösterir. Varsayılan değer HtmlLinkTargetType.Parent'dir. |
| [IsIECompatible](./isiecompatible/) | Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur. |
| [SetIsIECompatible](./setisiecompatible/) | Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur. |
| [GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | Hücre, sütunu aştığında tüm biçimlendirilmiş verinin gösterilip gösterilmeyeceğini gösterir. True ise sütun genişliği yok sayılır ve hücrenin tüm verisi dışa aktarılır. False ise veri Excel'deki gibi dışa aktarılır. Varsayılan değer false'tur. |
| [SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | Hücre, sütunu aştığında tüm biçimlendirilmiş verinin gösterilip gösterilmeyeceğini gösterir. True ise sütun genişliği yok sayılır ve hücrenin tüm verisi dışa aktarılır. False ise veri Excel'deki gibi dışa aktarılır. Varsayılan değer false'tur. |
| [GetCalculateFormula](./getcalculateformula/) | HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [SetCalculateFormula](./setcalculateformula/) | HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [IsJsBrowserCompatible](./isjsbrowsercompatible/) | JavaScript'in JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. Varsayılan değer true'dur. |
| [SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | JavaScript'in JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. Varsayılan değer true'dur. |
| [IsMobileCompatible](./ismobilecompatible/) | Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur. |
| [SetIsMobileCompatible](./setismobilecompatible/) | Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur. |
| [GetCssStyles](./getcssstyles/) | Biçimlendirici için ek CSS stillerini alır veya ayarlar. Yalnızca SaveAsSingleFile true olduğunda çalışır. |
| [SetCssStyles](./setcssstyles/) | Biçimlendirici için ek CSS stillerini alır veya ayarlar. Yalnızca SaveAsSingleFile true olduğunda çalışır. |
| [GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | Hücre biçimi satır içi kaydırma (wrap text) olarak ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | Hücre biçimi satır içi kaydırma (wrap text) olarak ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [IsBorderCollapsed](./isbordercollapsed/) | Tablo kenarlıklarının çöküp çökmediğini gösterir. Varsayılan değer true'dur. |
| [SetIsBorderCollapsed](./setisbordercollapsed/) | Tablo kenarlıklarının çöküp çökmediğini gösterir. Varsayılan değer true'dur. |
| [GetEncodeEntityAsCode](./getencodeentityascode/) | HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmediğini gösterir. (ör. "&amp;nbsp;" "&amp;#160;" ile değiştirilir). Varsayılan değer false'tur. |
| [SetEncodeEntityAsCode](./setencodeentityascode/) | HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmediğini gösterir. (ör. "&amp;nbsp;" "&amp;#160;" ile değiştirilir). Varsayılan değer false'tur. |
| [GetOfficeMathOutputMode](./getofficemathoutputmode/) | OfficeMath nesnelerinin HTML'ye nasıl dışa aktarıldığını gösterir. Varsayılan değer Image'dır. |
| [SetOfficeMathOutputMode](./setofficemathoutputmode/) | OfficeMath nesnelerinin HTML'ye nasıl dışa aktarıldığını gösterir. Varsayılan değer Image'dır. |
| [GetCellNameAttribute](./getcellnameattribute/) | Yazılacak CellName'i gösteren özniteliği belirtir. (ör. Değer "id" ise, "A1" hücresi için çıktı &lt;td id='A1'&gt; olur). Varsayılan değer null'dur. |
| [SetCellNameAttribute](./setcellnameattribute/) | Yazılacak CellName'i gösteren özniteliği belirtir. (ör. Değer "id" ise, "A1" hücresi için çıktı &lt;td id='A1'&gt; olur). Varsayılan değer null'dur. |
| [GetDisableCss](./getdisablecss/) | Yalnızca satır içi stillerin uygulanıp uygulanmadığını, CSS'ye dayanılmadan gösterir. Varsayılan değer false'tur. |
| [SetDisableCss](./setdisablecss/) | Yalnızca satır içi stillerin uygulanıp uygulanmadığını, CSS'ye dayanılmadan gösterir. Varsayılan değer false'tur. |
| [GetEnableCssCustomProperties](./getenablecsscustomproperties/) | HTML çıktısını CSS özel özellikleri kullanarak optimize eder. Örneğin, aynı base64 görüntünün birden çok kez kullanıldığı senaryoda, özel özellik sayesinde görüntü verisi yalnızca bir kez kaydedilir ve ortaya çıkan HTML'nin performansı artırılabilir. Varsayılan değer false'tur. |
| [SetEnableCssCustomProperties](./setenablecsscustomproperties/) | HTML çıktısını CSS özel özellikleri kullanarak optimize eder. Örneğin, aynı base64 görüntünün birden çok kez kullanıldığı senaryoda, özel özellik sayesinde görüntü verisi yalnızca bir kez kaydedilir ve ortaya çıkan HTML'nin performansı artırılabilir. Varsayılan değer false'tur. |
| [GetHtmlVersion](./gethtmlversion/) | HTML formatı kaydedilirken kullanılacak HTML standardı sürümünü belirtir. Varsayılan değer HtmlVersion.Default'tır. |
| [SetHtmlVersion](./sethtmlversion/) | HTML formatı kaydedilirken kullanılacak HTML standardı sürümünü belirtir. Varsayılan değer HtmlVersion.Default'tır. |
| [GetSheetSet](./getsheetset/) | Renderlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Renderlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetLayoutMode](./getlayoutmode/) | HTML'ye kaydederken düzen modunu alır veya ayarlar. Varsayılan değer HtmlLayoutMode.Normal'dır. |
| [SetLayoutMode](./setlayoutmode/) | HTML'ye kaydederken düzen modunu alır veya ayarlar. Varsayılan değer HtmlLayoutMode.Normal'dır. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | HTML dosyasına gömülecek yazı tipi dosyasının türünü alır veya ayarlar. Varsayılan değer HtmlEmbeddedFontType.None'dur ve bu, HTML'ye hiçbir yazı tipinin gömülmeyeceğini gösterir. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | HTML dosyasına gömülecek yazı tipi dosyasının türünü alır veya ayarlar. Varsayılan değer HtmlEmbeddedFontType.None'dur ve bu, HTML'ye hiçbir yazı tipinin gömülmeyeceğini gösterir. |
| [GetExportNamedRangeAnchors](./getexportnamedrangeanchors/) | HTML olarak kaydederken adlandırılmış aralıklar için bağlantı (anchor) öğelerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. |
| [SetExportNamedRangeAnchors](./setexportnamedrangeanchors/) | HTML olarak kaydederken adlandırılmış aralıklar için bağlantı (anchor) öğelerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. |
| [GetDataBarRenderMode](./getdatabarrendermode/) | Excel dosyalarını HTML dosyalarına dönüştürürken DataBar'ın nasıl render edileceği modunu temsil eder. Varsayılan değer DataBarRenderMode.BackgroundColor'dır. |
| [SetDataBarRenderMode](./setdatabarrendermode/) | Excel dosyalarını HTML dosyalarına dönüştürürken DataBar'ın nasıl render edileceği modunu temsil eder. Varsayılan değer DataBarRenderMode.BackgroundColor'dır. |
| [GetSpaceMode](./getspacemode/) | HTML çıktısında boşlukların nasıl render edildiğini gösterir. Bu seçenek şu anda yalnızca sayısal biçimlere (ör. muhasebe biçimi) uygulanır. Varsayılan değer HtmlSpaceMode.Css'tir. |
| [SetSpaceMode](./setspacemode/) | HTML çıktısında boşlukların nasıl render edildiğini gösterir. Bu seçenek şu anda yalnızca sayısal biçimlere (ör. muhasebe biçimi) uygulanır. Varsayılan değer HtmlSpaceMode.Css'tir. |
| [GetSaveFormat](./getsaveformat/) | Kaydetme dosya formatını alır. |
| [GetClearData](./getcleardata/) | Dosya kaydedildikten sonra çalışma kitabını boş bırak. |
| [SetClearData](./setcleardata/) | Dosya kaydedildikten sonra çalışma kitabını boş bırak. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [GetMergeAreas](./getmergeareas/) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [SetMergeAreas](./setmergeareas/) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [GetCreateDirectory](./getcreatedirectory/) | Doğruysa ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [SetCreateDirectory](./setcreatedirectory/) | Doğruysa ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [GetSortNames](./getsortnames/) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [SetSortNames](./setsortnames/) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [GetSortExternalNames](./getsortexternalnames/) | Dosya kaydedilmeden önce dış tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [SetSortExternalNames](./setsortexternalnames/) | Dosya kaydedilmeden önce dış tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Kaydedilirken .xls dosyası olarak belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer true'dur. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Kaydedilirken .xls dosyası olarak belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. Varsayılan değer true'dur. |
