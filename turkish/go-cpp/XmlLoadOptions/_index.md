---
title: "XmlLoadOptions Sınıfı"
linktitle: "XmlLoadOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "XmlLoadOptions sınıfı. Go dilinde xmlloadoptions nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/xmlloadoptions/
---

## XmlLoadOptions class

XML yükleme seçeneklerini temsil eder.

```go

type XmlLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewXmlLoadOptions](./newxmlloadoptions/) | XML dosyasını yükleme seçeneklerini temsil eder. |
| [NewXmlLoadOptions_LoadFormat](./newxmlloadoptions_loadformat/) | XML dosyasını yükleme seçeneklerini temsil eder. |
| [NewXmlLoadOptions_LoadOptions](./newxmlloadoptions_loadoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetStartCell](./getstartcell/) | Başlangıç hücresini alır ve ayarlar. |
| [SetStartCell](./setstartcell/) | Başlangıç hücresini alır ve ayarlar. |
| [IsXmlMap](./isxmlmap/) | XML'in Excel'e eşlenip eşlenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetIsXmlMap](./setisxmlmap/) | XML'in Excel'e eşlenip eşlenmeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetContainsMultipleWorksheets](./getcontainsmultipleworksheets/) | XML'in birden fazla çalışma sayfası olarak içe aktarılıp aktarılmayacağını gösterir. |
| [SetContainsMultipleWorksheets](./setcontainsmultipleworksheets/) | XML'in birden fazla çalışma sayfası olarak içe aktarılıp aktarılmayacağını gösterir. |
| [GetConvertNumericOrDate](./getconvertnumericordate/) | XML dosyasındaki değerin sayısal veya tarih biçimine dönüştürülüp dönüştürülmeyeceğini gösterir. |
| [SetConvertNumericOrDate](./setconvertnumericordate/) | XML dosyasındaki değerin sayısal veya tarih biçimine dönüştürülüp dönüştürülmeyeceğini gösterir. |
| [Get_NumberFormat](./get_numberformat/) | Sayısal değerin biçimini alır ve ayarlar. |
| [SetNumberFormat](./setnumberformat/) | Sayısal değerin biçimini alır ve ayarlar. |
| [Get_DateFormat](./get_dateformat/) | Tarih değerinin biçimini alır ve ayarlar. |
| [SetDateFormat](./setdateformat/) | Tarih değerinin biçimini alır ve ayarlar. |
| [GetIgnoreRootAttributes](./getignorerootattributes/) | Kök öğenin özniteliklerinin göz ardı edilip edilmeyeceğini gösterir. |
| [SetIgnoreRootAttributes](./setignorerootattributes/) | Kök öğenin özniteliklerinin göz ardı edilip edilmeyeceğini gösterir. |
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
