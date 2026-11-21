---
title: "HtmlSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "HTML dosyasını kaydetme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

HTML dosyasını kaydetme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | html dosyası kaydetmek için seçenekler oluşturur. |
| [HtmlSaveOptions(int saveFormat)](#HtmlSaveOptions-int-) | htm dosyası kaydetmek için seçenekler oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | CSS font-family'ye genel bir yazı tipi eklenip eklenmeyeceğini gösterir. |
| [getAddTooltipText()](#getAddTooltipText--) | Veri tam olarak görüntülenemediğinde araç ipucu metni eklenip eklenmeyeceğini gösterir. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Ekli dosyaların kaydedileceği dizin. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [getCalculateFormula()](#getCalculateFormula--) | HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [getCellCssPrefix()](#getCellCssPrefix--) | CSS adının önekini alır, varsayılan değer ""dır. |
| [getCellNameAttribute()](#getCellNameAttribute--) | Yazılacak CellName'i gösteren özelliği belirtir. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [getCreateDirectory()](#getCreateDirectory--) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [getCssStyles()](#getCssStyles--) | Biçimlendirici için ek CSS stillerini alır. |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | Excel dosyaları HTML dosyalarına dönüştürülürken DataBar'ın nasıl render edileceğini temsil eder. |
| [getDefaultFontName()](#getDefaultFontName--) | HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur. |
| [getDisableCss()](#getDisableCss--) | Yalnızca satır içi stillerin uygulanıp uygulanmayacağını, CSS'ye dayanılmadan gösterir. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Dosya HTML'ye dışa aktarılırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false'tur. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Yazı tipi dosyasının HTML dosyasına gömülme türünü alır. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | HTML çıktısını CSS özel özelliklerini kullanarak optimize eder. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmeyeceğini gösterir. |
| [getEncoding()](#getEncoding--) | Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Kullanılmayan stillerin dışarıda bırakılıp bırakılmayacağını gösterir. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Yalnızca etkin çalışma sayfasının HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportArea()](#getExportArea--) | Mevcut etkin Çalışma Sayfasının dışa aktarım CellArea'ını alır. |
| [getExportBogusRowData()](#getExportBogusRowData--) | Yanlış alt satır verilerinin dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | Dosya HTML'ye kaydedilirken boş olmayan hücrelerin Excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportCommentsType()](#getExportCommentsType--) | Yorumların HTML dosyalarına dışa aktarım türünü temsil eder. |
| [getExportDataOptions()](#getExportDataOptions--) | HTML dosyası verilerinin dışa aktarım kuralını gösterir. Varsayılan değer All'dir. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | Metin uzunluğu maksimum görüntüleme sütunundan uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportFormula()](#getExportFormula--) | Dosya HTML'ye kaydedilirken formüllerin dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | Çerçeve betikleri ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportGridLines()](#getExportGridLines--) | Izgara çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [getExportHeadings()](#getExportHeadings--) | HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Görüntülerin HTML, MHTML veya EPUB'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | HTML olarak kaydederken adlandırılmış aralıklar için bağlantı (anchor) öğelerinin dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportObjectListener()](#getExportObjectListener--) | Nesneleri dışa aktarmak için ExportObjectListener'ı alır. |
| [getExportPageFooters()](#getExportPageFooters--) | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Yazdırma alanının yalnızca HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Tarayıcılar tarafından desteklenmeyen kenarlık stilinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportSingleTab()](#getExportSingleTab--) | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Çalışma sayfası CSS'inin ayrı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [getFilePathProvider()](#getFilePathProvider--) | Çalışma sayfasını ayrı olarak HTML'ye dışa aktarmak için IFilePathProvider'ı alır. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | Sütun taşması durumunda hücrenin tüm biçimlendirilmiş verisinin gösterilip gösterilmeyeceğini gösterir. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Excel'de gizli sütun (bu sütunun genişliği 0) HTML formatına kaydetmeden önce, eğer HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya dahil edilmez, değer "Hidden" ise sütun çıktıya dahil edilir ancak gizli olarak kalır, varsayılan değer "Hidden"dır. |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Excel'de gizli satır (bu satırın yüksekliği 0) HTML formatına kaydetmeden önce, eğer HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya dahil edilmez, değer "Hidden" ise satır çıktıya dahil edilir ancak gizli olarak kalır, varsayılan değer "Hidden"dır. |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | Hücre biçimi satır içinde kaydırma (wrap text) olarak ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Excel dosyasını HTML formatında kaydederken hücreler arası bir dizeyin MS Excel'deki gibi görüntülenip görüntülenmeyeceğini gösterir. |
| [getHtmlVersion()](#getHtmlVersion--) | HTML formatını kaydederken kullanılacak HTML standardı sürümünü belirtir. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Görünür olmayan şekillerin dışa aktarılıp aktarılmayacağını belirtir |
| [getImageOptions()](#getImageOptions--) | Dışa aktarmadan önce ImageOrPrintOptions nesnesini al |
| [getImageScalable()](#getImageScalable--) | Sütun genişliğini ölçeklenebilir birimle tanımlarken görüntü genişliğini de ölçeklenebilir birimle tanımlayıp tanımlamayacağını gösterir. |
| [getLayoutMode()](#getLayoutMode--) | HTML'ye kaydederken düzen (layout) modunu alır. |
| [getLinkTargetType()](#getLinkTargetType--) | `<a>` bağlantısındaki hedef özniteliğin türünü belirtiyor. |
| [getMergeAreas()](#getMergeAreas--) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Dosya html'ye dışa aktarılırken boş TD öğesinin zorunlu bir şekilde birleştirilip birleştirilmeyeceğini gösterir. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | Ardışık boş hücreleri (boş td öğeleri) birleştirme seçeneği. Varsayılan değer MergeEmptyTdType.Default'tir. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | OfficeMath nesnelerinin HTML'ye nasıl dışa aktarıldığını gösterir, varsayılan değer Image'dır. |
| [getPageTitle()](#getPageTitle--) | HTML sayfasının başlığı. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Hücredeki html etiketi (örneğin `<div></div>`) hücre değeri olarak ayrıştırılmalı mı yoksa olduğu gibi korunmalı mı olduğunu gösterir. |
| [getPresentationPreference()](#getPresentationPreference--) | HTML veya mht dosyasının sunum tercihi olup olmadığını belirtiyor. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | HTML'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. |
| [getSaveFormat()](#getSaveFormat--) | Kaydetme dosya formatını alır. |
| [getSheetSet()](#getSheetSet--) | Render edilecek sayfaları alır. |
| [getShowAllSheets()](#getShowAllSheets--) | Tek bir HTML dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini belirtir. |
| [getSortExternalNames()](#getSortExternalNames--) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getSortNames()](#getSortNames--) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getSpaceMode()](#getSpaceMode--) | Boşlukların HTML çıktısında nasıl işlendiğini gösterir. |
| [getStreamProvider()](#getStreamProvider--) | Nesneleri dışa aktarmak için IStreamProvider'ı alır. |
| [getTableCssId()](#getTableCssId--) | tr, col, td gibi tip css adlarının önekini alır; bu önekler belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [getWidthScalable()](#getWidthScalable--) | Sütun genişliğinin ölçek birimiyle HTML'ye dışa aktarılıp aktarılmayacağını gösterir. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Dosya HTML'ye kaydedilirken çalışma sayfası yakınlaştırma seviyesine göre HTML'nin yakınlaştırılıp yakınlaştırılmayacağını gösterir, varsayılan değer false'tur. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | Tablo kenarlıklarının birleştirilip birleştirilmeyeceğini gösterir. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Görüntü dosyalarının geçici dizine dışa aktarılıp aktarılmayacağını gösterir. |
| [isExportComments()](#isExportComments--) | Dosya HTML'ye kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur. |
| [isFullPathLink()](#isFullPathLink--) | sheet00x.htm, filelist.xml ve tabstrip.htm dosyalarında tam yol bağlantısı kullanılıp kullanılmayacağını belirtiyor. |
| [isIECompatible()](#isIECompatible--) | Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını belirtiyor. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | JavaScript'in, JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. |
| [isMobileCompatible()](#isMobileCompatible--) | Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | CSS font-family'ye genel bir yazı tipi eklenip eklenmeyeceğini gösterir. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Veri tam olarak görüntülenemediğinde araç ipucu metni eklenip eklenmeyeceğini gösterir. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Ekli dosyaların kaydedileceği dizin. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | Tablo kenarlıklarının birleştirilip birleştirilmeyeceğini gösterir. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | CSS adının önekini ayarlar, varsayılan değer ""dır. |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | Yazılacak CellName'i gösteren özelliği belirtir. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setClearData(boolean value)](#setClearData-boolean-) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | Biçimlendirici için ek CSS stillerini ayarlar. |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | Excel dosyaları HTML dosyalarına dönüştürülürken DataBar'ın nasıl render edileceğini temsil eder. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | Yalnızca satır içi stillerin uygulanıp uygulanmayacağını, CSS'ye dayanılmadan gösterir. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Dosya HTML'ye dışa aktarılırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false'tur. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Yazı tipi dosyasının HTML dosyasına gömülme türünü ayarlar. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | HTML çıktısını CSS özel özelliklerini kullanarak optimize eder. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmeyeceğini gösterir. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini gösterir. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Kullanılmayan stillerin dışarıda bırakılıp bırakılmayacağını gösterir. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Görüntü dosyalarının geçici dizine dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Yalnızca etkin çalışma sayfasının HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Geçerli aktif Worksheet'ın dışa aktarma CellArea'sını ayarlar. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Yanlış alt satır verilerinin dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Dosya HTML'ye kaydedilirken boş olmayan hücrelerin Excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Dosya HTML'ye kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Yorumların HTML dosyalarına dışa aktarım türünü temsil eder. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | HTML dosyası verilerinin dışa aktarım kuralını gösterir. Varsayılan değer All'dir. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Metin uzunluğu maksimum görüntüleme sütunundan uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Dosya HTML'ye kaydedilirken formüllerin dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Çerçeve betikleri ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Izgara çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Görüntülerin HTML, MHTML veya EPUB'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir. |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | HTML olarak kaydederken adlandırılmış aralıklar için bağlantı (anchor) öğelerinin dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Nesneleri dışa aktarmak için ExportObjectListener'ı ayarlar. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Yazdırma alanının yalnızca HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Tarayıcılar tarafından desteklenmeyen kenarlık stilinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Çalışma sayfası CSS'inin ayrı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Worksheet'ı ayrı ayrı html'ye dışa aktarmak için IFilePathProvider'ı ayarlar. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | Sütun taşması durumunda hücrenin tüm biçimlendirilmiş verisinin gösterilip gösterilmeyeceğini gösterir. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | sheet00x.htm, filelist.xml ve tabstrip.htm dosyalarında tam yol bağlantısı kullanılıp kullanılmayacağını belirtiyor. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Excel'de gizli sütun (bu sütunun genişliği 0) HTML formatına kaydetmeden önce, eğer HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya dahil edilmez, değer "Hidden" ise sütun çıktıya dahil edilir ancak gizli olarak kalır, varsayılan değer "Hidden"dır. |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Excel'de gizli satır (bu satırın yüksekliği 0) HTML formatına kaydetmeden önce, eğer HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya dahil edilmez, değer "Hidden" ise satır çıktıya dahil edilir ancak gizli olarak kalır, varsayılan değer "Hidden"dır. |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | Hücre biçimi satır içinde kaydırma (wrap text) olarak ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Excel dosyasını HTML formatında kaydederken hücreler arası bir dizeyin MS Excel'deki gibi görüntülenip görüntülenmeyeceğini gösterir. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | HTML formatını kaydederken kullanılacak HTML standardı sürümünü belirtir. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını belirtiyor. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Görünür olmayan şekillerin dışa aktarılıp aktarılmayacağını belirtir |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Sütun genişliğini ölçeklenebilir birimle tanımlarken görüntü genişliğini de ölçeklenebilir birimle tanımlayıp tanımlamayacağını gösterir. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | JavaScript'in, JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. |
| [setLayoutMode(int value)](#setLayoutMode-int-) | HTML'ye kaydederken düzen modunu ayarlar. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | `<a>` bağlantısındaki hedef özniteliğin türünü belirtiyor. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Dosya html'ye dışa aktarılırken boş TD öğesinin zorunlu bir şekilde birleştirilip birleştirilmeyeceğini gösterir. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | Ardışık boş hücreleri (boş td öğeleri) birleştirme seçeneği. Varsayılan değer MergeEmptyTdType.Default'tir. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | OfficeMath nesnelerinin HTML'ye nasıl dışa aktarıldığını gösterir, varsayılan değer Image'dır. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | HTML sayfasının başlığı. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Hücredeki html etiketi (örneğin `<div></div>`) hücre değeri olarak ayrıştırılmalı mı yoksa olduğu gibi korunmalı mı olduğunu gösterir. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | HTML veya mht dosyasının sunum tercihi olup olmadığını belirtiyor. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir. |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | HTML'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Render edilecek sayfaları ayarlar. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Tek bir HTML dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini belirtir. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setSpaceMode(int value)](#setSpaceMode-int-) | Boşlukların HTML çıktısında nasıl işlendiğini gösterir. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Nesneleri dışa aktarmak için IStreamProvider'ı ayarlar. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | tr, col, td gibi tip css adlarının önekini ayarlar; bu önek, belirli TableCssId özniteliğine sahip tablo elemanında bulunur. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Akıllı sanat ayarının güncellenip güncellenmeyeceğini gösterir. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Sütun genişliğinin ölçek birimiyle HTML'ye dışa aktarılıp aktarılmayacağını gösterir. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Dosya HTML'ye kaydedilirken çalışma sayfası yakınlaştırma seviyesine göre HTML'nin yakınlaştırılıp yakınlaştırılmayacağını gösterir, varsayılan değer false'tur. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


html dosyası kaydetmek için seçenekler oluşturur.

### HtmlSaveOptions(int saveFormat) {#HtmlSaveOptions-int-}
```
public HtmlSaveOptions(int saveFormat)
```


htm dosyası kaydetmek için seçenekler oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Dosya formatı. Aşağıdaki türlerden biri olmalıdır: [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) veya [SaveFormat.M\_HTML](../../com.aspose.cells/saveformat\#M-HTML), aksi takdirde kaydedilen format otomatik olarak [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) olarak ayarlanır. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


CSS font-family'ye genel bir yazı tipi eklenip eklenmeyeceğini gösterir. Varsayılan değer true'tir.

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


Veri tam olarak görüntülenemediğinde araç ipucu metni eklenip eklenmeyeceğini gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Ekli dosyaların kaydedileceği dizin. Yalnızca html akışına kaydederken kullanılır.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Html dosyasındaki resim gibi ekli dosyaların Url önekini belirtin. Yalnızca html akışına kaydederken kullanılır.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör.

**Remarks**

Eğer klasör belirtilmemişse, varsayılan değeri [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)'dır. Eğer varsayılan değeri null veya boş ise, ya da null veya boş olarak belirtilmişse, çalışma kitabı kaydedilirken önbellek dosyası kullanılmaz.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


CSS adının önekini alır, varsayılan değer ""dır.

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


Yazılacak CellName'i gösteren özniteliği belirtir. (ör. Değer "id" ise, "A1" hücresi için çıktı <td id='A1'> olur). Varsayılan değer null'dır.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarını kontrol edip etmeyeceği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girdiğinizde, kesilir.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Dosya kaydedildikten sonra çalışma kitabını boşalt.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


Biçimlendirici için ek css stillerini alır. Yalnızca [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) true olduğunda çalışır. CssStyles="body \{ padding: 5px \}";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


Excel dosyalarını html dosyalarına dönüştürürken DataBar'ın nasıl render edileceğini temsil eder. Varsayılan değer [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

[DataBarRenderMode](../../com.aspose.cells/databarrendermode)'a bakın.

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur.

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


CSS'e dayanılmadan yalnızca satır içi stillerin uygulanıp uygulanmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


Dosya HTML'ye dışa aktarılırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false'tur.

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Yazı tipi dosyasının html dosyasına gömülme türünü alır. Varsayılan değer [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) olup, html'e hiçbir yazı tipinin gömülmeyeceğini gösterir.

[HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype)'a bakın.

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


HTML çıktısını CSS özel özellikleri kullanarak optimize eder. Örneğin, aynı base64 görüntünün birden çok kez kullanıldığı senaryoda, özel özellik sayesinde görüntü verisi yalnızca bir kez kaydedilir ve ortaya çıkan HTML'in performansı artırılır. Varsayılan değer false'tur.

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmediğini gösterir. (ör. "&nbsp;" "&\#160;" ile değiştirilir). Varsayılan değer false'tur.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini belirtir. Varsayılan değer true'tur.

**Remarks**

Yalnızca .xls, .xlsx, .xlsb ve .xlsm dosyaları için.

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


Kullanılmayan stillerin dışlanıp dışlanmayacağını gösterir. Oluşturulan html dosyalarında kullanılmayan stillerin dışlanması, görsel etkilere zarar vermeden dosya boyutunu küçültebilir. Bu nedenle bu özelliğin varsayılan değeri true'tır. Kullanıcı, oluşturulan html için çalışma kitabındaki tüm stilleri (ör. çalışma kitabını daha sonra html'den geri yükleme senaryosu) tutmak istiyorsa, lütfen bu özelliği false olarak ayarlayın.

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Yalnızca aktif çalışma sayfasının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. True ise sadece aktif çalışma sayfası html dosyasına dışa aktarılır; False ise tüm çalışma kitabı html dosyasına dışa aktarılır. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Geçerli aktif Worksheet'ın dışa aktarma CellArea'sını alır. Bu özniteliği ayarlarsanız, geçerli aktif Worksheet'ın yazdırma alanı atlanır. Dosya html olarak kaydedildiğinde yalnızca belirtilen alan dışa aktarılır.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


Sağlam olmayan alt satır verisinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. Html veya mht dosyasını excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


Dosya html olarak kaydedilirken boş olmayan hücrelerin excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Çıktı html'yi excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


Yorumların HTML dosyalarına dışa aktarım türünü temsil eder.

Bakınız [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


HTML dosyası verilerinin dışa aktarım kuralını gösterir. Varsayılan değer All'dir.

Bakınız [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


Metin uzunluğu maksimum gösterim sütunundan daha uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Html dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


Dosya html olarak kaydedilirken formüllerin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. Çıktı html'yi excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


Çerçeve betikleri ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. Html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Izgara çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen HtmlSaveOptions.ExportRowColumnHeadings özelliğini kullanın. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Görüntülerin HTML, MHTML veya EPUB'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir.

**Remarks**

Bu özellik true olarak ayarlandığında görüntü verileri doğrudan img öğelerine dışa aktarılır ve ayrı dosyalar oluşturulmaz.

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


HTML olarak kaydedilirken adlandırılmış aralıklar için bağlantı (anchor) öğelerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tir.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


Nesneleri dışa aktarmak için ExportObjectListener'ı alır.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen HtmlSaveOptions.IStreamProvider özelliğini kullanın. Bu özellik, Ağustos 2015'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Yalnızca [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\\#getSaveAsSingleFile--) true olduğunda çalışır.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Yalnızca [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\\#getSaveAsSingleFile--) true olduğunda çalışır.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Yalnızca yazdırma alanının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


Tarayıcılar tarafından desteklenmeyen kenarlık stilinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını gösterir. Html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


Çalışma sayfası CSS'inin ayrı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


Çalışma sayfasını ayrı olarak HTML'ye dışa aktarmak için IFilePathProvider'ı alır.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


Sütunu aşan hücredeki tüm biçimlendirilmiş verinin gösterilip gösterilmeyeceğini belirler. True ise sütun genişliği göz ardı edilir ve hücrenin tüm verisi dışa aktarılır. False ise veri Excel gibi dışa aktarılır. Varsayılan değer false'tur.

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


Excel'de gizli sütun (bu sütunun genişliği 0) HTML formatına kaydetmeden önce, eğer HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya dahil edilmez, değer "Hidden" ise sütun çıktıya dahil edilir ancak gizli olarak kalır, varsayılan değer "Hidden"dır.

Bakınız [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


Excel'de gizli satır (bu satırın yüksekliği 0) HTML formatına kaydetmeden önce, eğer HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya dahil edilmez, değer "Hidden" ise satır çıktıya dahil edilir ancak gizli olarak kalır, varsayılan değer "Hidden"dır.

Bakınız [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


Hücre biçimi metni kaydıracak şekilde ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. Varsayılan değer false'tur

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


Excel dosyasını html formatında kaydederken çapraz hücre dizgisinin MS Excel ile aynı şekilde görüntülenip görüntülenmeyeceğini gösterir. Varsayılan değer Default'tır, bu nedenle çapraz hücre dizgileri için Aspose.Cells ve MS Excel tarafından oluşturulan html dosyaları arasında çok az fark vardır. Ancak büyük html dosyaları oluşturma performansı açısından, değeri Cross olarak ayarlamak, Default veya Fit2Cell olarak ayarlamaktan birkaç kat daha hızlı olur.

Bakınız [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


HTML formatı kaydedilirken kullanılacak HTML standardı sürümünü belirtir. Varsayılan değer HtmlVersion.Default'tir.

Bakınız [HtmlVersion](../../com.aspose.cells/htmlversion).

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


Görünür olmayan şekillerin dışa aktarılıp aktarılmayacağını belirtir

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Dışa aktarmadan önce ImageOrPrintOptions nesnesini al

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


Sütun genişliğini tanımlamak için ölçeklenebilir birim kullanılırken görüntü genişliğini tanımlamak için ölçeklenebilir birim kullanılıp kullanılmayacağını gösterir. Varsayılan değer true'tur.

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


HTML olarak kaydedilirken düzen (layout) modunu alır. Varsayılan değer [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\\#NORMAL)'dır.

Bakınız [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


`<a>` bağlantısındaki hedef özniteliğinin türünü belirtir. Varsayılan değer HtmlLinkTargetType.Parent.

Bakınız [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


HTML dosyasına dışa aktarırken boş TD öğesinin zorunlu birleştirilip birleştirilmeyeceğini gösterir. Değer true olarak ayarlandığında HTML dosyasının boyutu önemli ölçüde azalır. Varsayılan değer false'tur. HTML dosyasını Excel'e içe aktarmak veya dosyayı HTML olarak kaydederken mükemmel ızgara çizgileri dışa aktarmak istiyorsanız, varsayılan değeri koruyun.

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


Ardışık boş hücreleri (boş td öğeleri) birleştirme seçeneği. Varsayılan değer MergeEmptyTdType.Default'tir.

Bakınız [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


OfficeMath nesnelerinin HTML'ye nasıl dışa aktarıldığını gösterir, varsayılan değer Image'dır.

Bakınız [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


HTML sayfasının başlığı. Yalnızca HTML akışına kaydetmek için.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Hücredeki HTML etiketi (ör. `<div></div>`) hücre değeri olarak ayrıştırılsın mı yoksa olduğu gibi korunsun mu olduğunu gösterir. Varsayılan değer true'tur.

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


HTML veya MHT dosyasının sunum tercihi olup olmadığını belirtir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız, değeri true olarak ayarlayın.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir.

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


HTML'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan değer false'tur.

**Remarks**

Çalışma kitabında birden fazla çalışma sayfası veya resimler gibi diğer gerekli kaynaklar varsa, genellikle bu çalışma sayfaları ve diğer kaynaklar ayrı dosyalara kaydedilir. Bazı senaryolarda, kullanıcı taşıma kolaylığı için yalnızca bir sonuç dosyası almak isteyebilir. Böyle bir durumda, kullanıcı bu özelliği true olarak ayarlayabilir.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Kaydetme dosya formatını alır.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Render edilecek sayfaları alır. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


Tek bir HTML dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini belirtir.

**Remarks**

Yalnızca [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\\#getSaveAsSingleFile--) true olduğunda çalışır.

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Returns:**
boolean
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


HTML çıktısında boşlukların nasıl render edildiğini gösterir. Bu seçenek şu anda yalnızca sayısal biçimlere (ör. muhasebe biçimi) uygulanır. Varsayılan değer [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Bakınız [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Nesneleri dışa aktarmak için IStreamProvider'ı alır.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


tr, col, td gibi tip CSS adlarının önekini alır; bu önek, belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. Varsayılan değer "".

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Akıllı sanat ayarının güncellenip güncellenmeyeceğini belirtir. Varsayılan değer false'tur.

**Remarks**

Yalnızca Shape.GetResultOfSmartArt() yöntemi çağrıldıktan ve önbelleğe alınmış şekiller şablon dosyasında mevcut olduğunda etkili olur.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Uyarı geri çağrısını alır.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


Sütun genişliğinin ölçek birimiyle HTML'ye dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


Dosya HTML'ye kaydedilirken çalışma sayfası yakınlaştırma seviyesine göre HTML'nin yakınlaştırılıp yakınlaştırılmayacağını gösterir, varsayılan değer false'tur.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBorderCollapsed() {#isBorderCollapsed--}
```
public boolean isBorderCollapsed()
```


Tablo kenarlıklarının çökertilip çökertilmeyeceğini gösterir. Varsayılan değer true'tur.

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


Görüntü dosyalarının geçici dizine dışa aktarılıp aktarılmayacağını gösterir. Yalnızca HTML akışına kaydetmek için.

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Dosya HTML'ye kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


sheet00x.htm, filelist.xml ve tabstrip.htm dosyalarında tam yol bağlantısı kullanılıp kullanılmayacağını belirtir. Varsayılan değer false'tur.

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını belirtir. Varsayılan değer false'tur.

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


JavaScript'in, JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. Varsayılan değer true'tur.

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAddGenericFont(boolean value) {#setAddGenericFont-boolean-}
```
public void setAddGenericFont(boolean value)
```


CSS font-family'ye genel bir yazı tipi eklenip eklenmeyeceğini gösterir. Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


Veri tam olarak görüntülenemediğinde araç ipucu metni eklenip eklenmeyeceğini gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Ekli dosyaların kaydedileceği dizin. Yalnızca html akışına kaydederken kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Html dosyasındaki resim gibi ekli dosyaların Url önekini belirtin. Yalnızca html akışına kaydederken kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


Tablo kenarlıklarının çökertilip çökertilmeyeceğini gösterir. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör.

**Remarks**

Eğer klasör belirtilmemişse, varsayılan değeri [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)'dır. Eğer varsayılan değeri null veya boş ise, ya da null veya boş olarak belirtilmişse, çalışma kitabı kaydedilirken önbellek dosyası kullanılmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


CSS adının önekini ayarlar, varsayılan değer ""dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


Yazılacak CellName'i gösteren özniteliği belirtir. (ör. Değer "id" ise, "A1" hücresi için çıktı <td id='A1'> olur). Varsayılan değer null'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarını kontrol edip etmeyeceği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girdiğinizde, kesilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Dosya kaydedildikten sonra çalışma kitabını boşalt.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


Biçimlendirici için ek CSS stillerini ayarlar. Yalnızca [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True olduğunda çalışır.  CssStyles="body \{ padding: 5px \}";

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


Excel dosyalarını html dosyalarına dönüştürürken DataBar'ın nasıl render edileceğini temsil eder. Varsayılan değer [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

[DataBarRenderMode](../../com.aspose.cells/databarrendermode)'a bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


CSS'e dayanılmadan yalnızca satır içi stillerin uygulanıp uygulanmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


Dosya HTML'ye dışa aktarılırken Downlevel-revealed koşullu yorumların devre dışı bırakılıp bırakılmayacağını gösterir, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


HTML dosyasına gömülecek yazı tipi dosyasının türünü ayarlar. Varsayılan değer [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) olup, HTML'ye hiçbir yazı tipinin gömülmeyeceğini gösterir.

[HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype)'a bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


HTML çıktısını CSS özel özellikleri kullanarak optimize eder. Örneğin, aynı base64 görüntünün birden çok kez kullanıldığı senaryoda, özel özellik sayesinde görüntü verisi yalnızca bir kez kaydedilir ve ortaya çıkan HTML'in performansı artırılır. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


HTML karakter varlıklarının ondalık kodla değiştirilip değiştirilmediğini gösterir. (ör. "&nbsp;" "&\#160;" ile değiştirilir). Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Bir .xls dosyası olarak kaydederken belge özelliklerinin şifrelenip şifrelenmeyeceğini belirtir. Varsayılan değer true'tur.

**Remarks**

Yalnızca .xls, .xlsx, .xlsb ve .xlsm dosyaları için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


Kullanılmayan stillerin dışlanıp dışlanmayacağını gösterir. Oluşturulan html dosyalarında kullanılmayan stillerin dışlanması, görsel etkilere zarar vermeden dosya boyutunu küçültebilir. Bu nedenle bu özelliğin varsayılan değeri true'tır. Kullanıcı, oluşturulan html için çalışma kitabındaki tüm stilleri (ör. çalışma kitabını daha sonra html'den geri yükleme senaryosu) tutmak istiyorsa, lütfen bu özelliği false olarak ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


Görüntü dosyalarının geçici dizine dışa aktarılıp aktarılmayacağını gösterir. Yalnızca HTML akışına kaydetmek için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Yalnızca aktif çalışma sayfasının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. True ise sadece aktif çalışma sayfası html dosyasına dışa aktarılır; False ise tüm çalışma kitabı html dosyasına dışa aktarılır. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Mevcut aktif Çalışma Sayfasının dışa aktarılacak CellArea'sını ayarlar. Bu özniteliği ayarlarsanız, mevcut aktif Çalışma Sayfasının yazdırma alanı atlanır. Dosya HTML olarak kaydedilirken yalnızca belirtilen alan dışa aktarılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


Sağlam olmayan alt satır verisinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. Html veya mht dosyasını excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


Dosya html olarak kaydedilirken boş olmayan hücrelerin excel koordinatlarının dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Çıktı html'yi excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Dosya HTML'ye kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


Yorumların HTML dosyalarına dışa aktarım türünü temsil eder.

Bakınız [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


HTML dosyası verilerinin dışa aktarım kuralını gösterir. Varsayılan değer All'dir.

Bakınız [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


Belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


Metin uzunluğu maksimum gösterim sütunundan daha uzun olduğunda ekstra başlıkların dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Html dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


Dosya html olarak kaydedilirken formüllerin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. Çıktı html'yi excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


Çerçeve betikleri ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. Html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Izgara çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen HtmlSaveOptions.ExportRowColumnHeadings özelliğini kullanın. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Görüntülerin HTML, MHTML veya EPUB'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir.

**Remarks**

Bu özellik true olarak ayarlandığında görüntü verileri doğrudan img öğelerine dışa aktarılır ve ayrı dosyalar oluşturulmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


HTML olarak kaydedilirken adlandırılmış aralıklar için bağlantı (anchor) öğelerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


Nesneleri dışa aktarmak için ExportObjectListener'ı ayarlar.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen HtmlSaveOptions.IStreamProvider özelliğini kullanın. Bu özellik, Ağustos 2015'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Yalnızca [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\\#getSaveAsSingleFile--) true olduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


Sayfa başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Yalnızca [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\\#getSaveAsSingleFile--) true olduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Yalnızca yazdırma alanının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


HTML dosyalarına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


Tarayıcılar tarafından desteklenmeyen kenarlık stilinde benzer kenarlık stilinin dışa aktarılıp aktarılmayacağını gösterir. Html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


Çalışma sayfası CSS'inin ayrı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


Worksheet'ı ayrı ayrı html'ye dışa aktarmak için IFilePathProvider'ı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


Sütunu aşan hücredeki tüm biçimlendirilmiş verinin gösterilip gösterilmeyeceğini belirler. True ise sütun genişliği göz ardı edilir ve hücrenin tüm verisi dışa aktarılır. False ise veri Excel gibi dışa aktarılır. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


sheet00x.htm, filelist.xml ve tabstrip.htm dosyalarında tam yol bağlantısı kullanılıp kullanılmayacağını belirtir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


Excel'de gizli sütun (bu sütunun genişliği 0) HTML formatına kaydetmeden önce, eğer HtmlHiddenColDisplayType "Remove" ise gizli sütun çıktıya dahil edilmez, değer "Hidden" ise sütun çıktıya dahil edilir ancak gizli olarak kalır, varsayılan değer "Hidden"dır.

Bakınız [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


Excel'de gizli satır (bu satırın yüksekliği 0) HTML formatına kaydetmeden önce, eğer HtmlHiddenRowDisplayType "Remove" ise gizli satır çıktıya dahil edilmez, değer "Hidden" ise satır çıktıya dahil edilir ancak gizli olarak kalır, varsayılan değer "Hidden"dır.

Bakınız [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


Hücre biçimi metni kaydıracak şekilde ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. Varsayılan değer false'tur

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


Excel dosyasını html formatında kaydederken çapraz hücre dizgisinin MS Excel ile aynı şekilde görüntülenip görüntülenmeyeceğini gösterir. Varsayılan değer Default'tır, bu nedenle çapraz hücre dizgileri için Aspose.Cells ve MS Excel tarafından oluşturulan html dosyaları arasında çok az fark vardır. Ancak büyük html dosyaları oluşturma performansı açısından, değeri Cross olarak ayarlamak, Default veya Fit2Cell olarak ayarlamaktan birkaç kat daha hızlı olur.

Bakınız [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


HTML formatı kaydedilirken kullanılacak HTML standardı sürümünü belirtir. Varsayılan değer HtmlVersion.Default'tir.

Bakınız [HtmlVersion](../../com.aspose.cells/htmlversion).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


Çıktı HTML'nin IE tarayıcısıyla uyumlu olup olmadığını belirtir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


Görünür olmayan şekillerin dışa aktarılıp aktarılmayacağını belirtir

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


Sütun genişliğini tanımlamak için ölçeklenebilir birim kullanılırken görüntü genişliğini tanımlamak için ölçeklenebilir birim kullanılıp kullanılmayacağını gösterir. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


JavaScript'in, JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


HTML olarak kaydederken düzen modunu ayarlar. Varsayılan değer [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Bakınız [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


`<a>` bağlantısındaki hedef özniteliğinin türünü belirtir. Varsayılan değer HtmlLinkTargetType.Parent.

Bakınız [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


HTML dosyasına dışa aktarırken boş TD öğesinin zorunlu birleştirilip birleştirilmeyeceğini gösterir. Değer true olarak ayarlandığında HTML dosyasının boyutu önemli ölçüde azalır. Varsayılan değer false'tur. HTML dosyasını Excel'e içe aktarmak veya dosyayı HTML olarak kaydederken mükemmel ızgara çizgileri dışa aktarmak istiyorsanız, varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


Ardışık boş hücreleri (boş td öğeleri) birleştirme seçeneği. Varsayılan değer MergeEmptyTdType.Default'tir.

Bakınız [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


Çıktı HTML'nin mobil cihazlarla uyumlu olup olmadığını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


OfficeMath nesnelerinin HTML'ye nasıl dışa aktarıldığını gösterir, varsayılan değer Image'dır.

Bakınız [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


HTML sayfasının başlığı. Yalnızca HTML akışına kaydetmek için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Hücredeki HTML etiketi (ör. `<div></div>`) hücre değeri olarak ayrıştırılsın mı yoksa olduğu gibi korunsun mu olduğunu gösterir. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


HTML veya MHT dosyasının sunum tercihi olup olmadığını belirtir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız, değeri true olarak ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Grafiğin en son verilerinin önbelleğe alınıp alınmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


HTML'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan değer false'tur.

**Remarks**

Çalışma kitabında birden fazla çalışma sayfası veya resimler gibi diğer gerekli kaynaklar varsa, genellikle bu çalışma sayfaları ve diğer kaynaklar ayrı dosyalara kaydedilir. Bazı senaryolarda, kullanıcı taşıma kolaylığı için yalnızca bir sonuç dosyası almak isteyebilir. Böyle bir durumda, kullanıcı bu özelliği true olarak ayarlayabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Render edilecek sayfaları ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


Tek bir HTML dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmeyeceğini belirtir.

**Remarks**

Yalnızca [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\\#getSaveAsSingleFile--) true olduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Dosya kaydedilmeden önce harici tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


HTML çıktısında boşlukların nasıl render edildiğini gösterir. Bu seçenek şu anda yalnızca sayısal biçimlere (ör. muhasebe biçimi) uygulanır. Varsayılan değer [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Bakınız [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Nesneleri dışa aktarmak için IStreamProvider'ı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


tr, col, td vb. gibi tip css adının önekini ayarlar, bunlar belirli TableCssId özniteliğine sahip tablo öğesinde bulunur. Varsayılan değer "".

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Akıllı sanat ayarının güncellenip güncellenmeyeceğini belirtir. Varsayılan değer false'tur.

**Remarks**

Yalnızca Shape.GetResultOfSmartArt() yöntemi çağrıldıktan ve önbelleğe alınmış şekiller şablon dosyasında mevcut olduğunda etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Uyarı geri çağrısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


Sütun genişliğinin ölçek birimiyle HTML'ye dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


Dosya HTML'ye kaydedilirken çalışma sayfası yakınlaştırma seviyesine göre HTML'nin yakınlaştırılıp yakınlaştırılmayacağını gösterir, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

