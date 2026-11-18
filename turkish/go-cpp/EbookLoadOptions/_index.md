---
title: "EbookLoadOptions Sınıfı"
linktitle: "EbookLoadOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "EbookLoadOptions sınıfı. Go'da ebookloadoptions'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/ebookloadoptions/
---

## EbookLoadOptions class

Bir e-kitap dosyası içe aktarılırken seçenekleri temsil eder.

```go

type EbookLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewEbookLoadOptions](./newebookloadoptions/) | E-kitap dosyasını yüklemek için bir seçenek oluşturur. |
| [NewEbookLoadOptions_LoadFormat](./newebookloadoptions_loadformat/) | E-kitap dosyasını yükleme seçeneği oluşturur. |
| [NewEbookLoadOptions_HtmlLoadOptions](./newebookloadoptions_htmlloadoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetEncoding](./getencoding/) | Varsayılan kodlamayı alır ve ayarlar. Yalnızca csv dosyası için geçerlidir. |
| [SetEncoding](./setencoding/) | Varsayılan kodlamayı alır ve ayarlar. Yalnızca csv dosyası için geçerlidir. |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrıştırılan değerler için uygulanacak stili gösteren stratejiyi belirtir. |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrıştırılan değerler için uygulanacak stili gösteren stratejiyi belirtir. |
| [GetConvertNumericData](./getconvertnumericdata/) | Metin dosyasındaki dizenin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [SetConvertNumericData](./setconvertnumericdata/) | Metin dosyasındaki dizenin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | Metin dosyasındaki dizenin tarih verisine dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | Metin dosyasındaki dizenin tarih verisine dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [GetKeepPrecision](./getkeepprecision/) | Uzunluğu 15 ise dize değerinin ayrıştırılmayacağını gösterir. |
| [SetKeepPrecision](./setkeepprecision/) | Uzunluğu 15 ise dize değerinin ayrıştırılmayacağını gösterir. |
| [GetLoadFormulas](./getloadformulas/) | Orijinal html dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir. |
| [SetLoadFormulas](./setloadformulas/) | Orijinal html dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir. |
| [GetSupportDivTag](./getsupportdivtag/) | Html dosyası <c>&lt;div&gt;</c> etiketini içerdiğinde bu etiketin düzenini destekleyip desteklemeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetSupportDivTag](./setsupportdivtag/) | Html dosyası <c>&lt;div&gt;</c> etiketini içerdiğinde bu etiketin düzenini destekleyip desteklemeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetDeleteRedundantSpaces](./getdeleteredundantspaces/) | Metin <c>&lt;br&gt;</c> etiketiyle satırları sararken gereksiz boşlukların silinip silinmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetDeleteRedundantSpaces](./setdeleteredundantspaces/) | Metin <c>&lt;br&gt;</c> etiketiyle satırları sararken gereksiz boşlukların silinip silinmeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetAutoFitColsAndRows](./getautofitcolsandrows/) | Sütunların ve satırların otomatik sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetAutoFitColsAndRows](./setautofitcolsandrows/) | Sütunların ve satırların otomatik sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur. |
| [GetHasFormula](./gethasformula/) | Metnin "=" ile başlıyorsa formül olup olmadığını gösterir. |
| [SetHasFormula](./sethasformula/) | Metnin "=" ile başlıyorsa formül olup olmadığını gösterir. |
| [GetProgId](./getprogid/) | Dosyayı oluşturan program kimliğini alır. Yalnızca MHT dosyaları için. |
| [GetTableLoadOptions](./gettableloadoptions/) | HtmlTableLoadOptionCollection örneğini al |
| [GetDetectLaTeX](./getdetectlatex/) | HTML dosyasında LaTeX formülünün algılanıp algılanmayacağını gösterir. Varsayılan değer false'tur. |
| [SetDetectLaTeX](./setdetectlatex/) | HTML dosyasında LaTeX formülünün algılanıp algılanmayacağını gösterir. Varsayılan değer false'tur. |
| [GetParagraphLayoutMode](./getparagraphlayoutmode/) | HTML yüklenirken &lt;p&gt; öğelerinin nasıl işleneceğini belirtir. Varsayılan değer HtmlParagraphLayoutMode.Normal'dur. |
| [SetParagraphLayoutMode](./setparagraphlayoutmode/) | HTML yüklenirken &lt;p&gt; öğelerinin nasıl işleneceğini belirtir. Varsayılan değer HtmlParagraphLayoutMode.Normal'dur. |
| [GetHyperlinkLoadMode](./gethyperlinkloadmode/) | HTML yüklenirken köprülerin nasıl yükleneceğini belirtir. |
| [SetHyperlinkLoadMode](./sethyperlinkloadmode/) | HTML yüklenirken köprülerin nasıl yükleneceğini belirtir. |
| [GetLoadFormat](./getloadformat/) | Yükleme biçimini alır. |
| [GetPassword](./getpassword/) | Çalışma kitabının şifresini alır ve ayarlar. |
| [SetPassword](./setpassword/) | Çalışma kitabının şifresini alır ve ayarlar. |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir. |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir. |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur. |
| [SetPaperSize](./setpapersize/) | Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar. |
| [GetLanguageCode](./getlanguagecode/) | Dosyanın kaydedildiği CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar. |
| [SetLanguageCode](./setlanguagecode/) | Dosyanın kaydedildiği CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar. |
| [GetRegion](./getregion/) | Yüklenmekte olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar. |
| [SetRegion](./setregion/) | Yüklenmekte olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Workbook stillerini başlatmak için varsayılan stil ayarlarını alır. |
| [GetInterruptMonitor](./getinterruptmonitor/) | Kesinti izleyicisini alır ve ayarlar. |
| [SetInterruptMonitor](./setinterruptmonitor/) | Kesinti izleyicisini alır ve ayarlar. |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar. |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar. |
| [GetCheckDataValid](./getcheckdatavalid/) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [SetCheckDataValid](./setcheckdatavalid/) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir Exception alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen hatalar oluşabilir. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir Exception alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen hatalar oluşabilir. |
| [GetKeepUnparsedData](./getkeepunparseddata/) | Workbook bir şablon dosyasından yüklendiğinde ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirtir. Varsayılan true'tur. |
| [SetKeepUnparsedData](./setkeepunparseddata/) | Workbook bir şablon dosyasından yüklendiğinde ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirtir. Varsayılan true'tur. |
| [GetLoadFilter](./getloadfilter/) | Verilerin nasıl yükleneceğini belirten filtre. |
| [SetLoadFilter](./setloadfilter/) | Verilerin nasıl yükleneceğini belirten filtre. |
| [GetMemorySetting](./getmemorysetting/) | Yüklenen workbook için bellek modunu alır veya ayarlar. |
| [SetMemorySetting](./setmemorysetting/) | Yüklenen workbook için bellek modunu alır veya ayarlar. |
| [GetAutoFitterOptions](./getautofitteroptions/) | Otomatik sığdırıcı seçeneklerini alır ve ayarlar. |
| [SetAutoFitterOptions](./setautofitteroptions/) | Otomatik sığdırıcı seçeneklerini alır ve ayarlar. |
| [GetAutoFilter](./getautofilter/) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir. |
| [SetAutoFilter](./setautofilter/) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir. |
| [GetFontConfigs](./getfontconfigs/) | Bireysel yazı tipi yapılandırmalarını alır ve ayarlar. Yalnızca bu LoadOptions ile yüklenen Workbook için çalışır. |
| [SetFontConfigs](./setfontconfigs/) | Bireysel yazı tipi yapılandırmalarını alır ve ayarlar. Yalnızca bu LoadOptions ile yüklenen Workbook için çalışır. |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | Gereksiz şekillerin yoksayılıp yoksayılmayacağını gösterir. |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | Gereksiz şekillerin yoksayılıp yoksayılmayacağını gösterir. |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | Formül tokenları arasında doldurulan boşluk ve satır sonlarının formüller alınırken ve ayarlanırken korunup korunmayacağını gösterir. Varsayılan değer false'tur. |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | Formül tokenları arasında doldurulan boşluk ve satır sonlarının formüller alınırken ve ayarlanırken korunup korunmayacağını gösterir. Varsayılan değer false'tur. |
