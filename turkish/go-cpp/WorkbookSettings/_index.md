---
title: "WorkbookSettings Sınıfı"
linktitle: "WorkbookSettings"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "WorkbookSettings sınıfı. Go'da workbooksettings'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/workbooksettings/
---

## WorkbookSettings class

Çalışma kitabının tüm ayarlarını temsil eder.

```go

type WorkbookSettings struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [Dispose](./dispose/) | Kaynakları serbest bırakır. |
| [GetThemeFont](./getthemefont/) | Varsayılan tema yazı tipi adını alır. |
| [GetAuthor](./getauthor/) | Dosyanın yazarını alır ve ayarlar. |
| [SetAuthor](./setauthor/) | Dosyanın yazarını alır ve ayarlar. |
| [GetCheckCustomNumberFormat](./getcheckcustomnumberformat/) | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini gösterir. |
| [SetCheckCustomNumberFormat](./setcheckcustomnumberformat/) | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini gösterir. |
| [GetEnableMacros](./getenablemacros/) | Makroları etkinleştir; |
| [SetEnableMacros](./setenablemacros/) | Makroları etkinleştir; |
| [GetDate1904](./getdate1904/) | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır veya ayarlar. |
| [SetDate1904](./setdate1904/) | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır veya ayarlar. |
| [GetProtectionType](./getprotectiontype/) | Çalışma kitabının koruma türünü alır. |
| [GetDisplayDrawingObjects](./getdisplaydrawingobjects/) | Çalışma kitabında nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini belirtir. |
| [SetDisplayDrawingObjects](./setdisplaydrawingobjects/) | Çalışma kitabında nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini belirtir. |
| [GetSheetTabBarWidth](./getsheettabbarwidth/) | Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'i cinsinden). |
| [SetSheetTabBarWidth](./setsheettabbarwidth/) | Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'i cinsinden). |
| [GetShowTabs](./getshowtabs/) | Çalışma kitabı sekmelerinin görüntülenip görüntülenmeyeceğini belirten bir değeri alır veya ayarlar. |
| [SetShowTabs](./setshowtabs/) | Çalışma kitabı sekmelerinin görüntülenip görüntülenmeyeceğini belirten bir değeri alır veya ayarlar. |
| [GetFirstVisibleTab](./getfirstvisibletab/) | İlk görünen çalışma sayfası sekmesini alır veya ayarlar. |
| [SetFirstVisibleTab](./setfirstvisibletab/) | İlk görünen çalışma sayfası sekmesini alır veya ayarlar. |
| [IsHScrollBarVisible](./ishscrollbarvisible/) | Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri alır veya ayarlar. |
| [SetIsHScrollBarVisible](./setishscrollbarvisible/) | Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri alır veya ayarlar. |
| [IsVScrollBarVisible](./isvscrollbarvisible/) | Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri alır veya ayarlar. |
| [SetIsVScrollBarVisible](./setisvscrollbarvisible/) | Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri alır veya ayarlar. |
| [GetShared](./getshared/) | Çalışma kitabının paylaşılıp paylaşılmadığını gösteren bir değeri alır veya ayarlar. |
| [SetShared](./setshared/) | Çalışma kitabının paylaşılıp paylaşılmadığını gösteren bir değeri alır veya ayarlar. |
| [GetLanguageCode](./getlanguagecode/) | Dosyanın kaydedildiği CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar. |
| [SetLanguageCode](./setlanguagecode/) | Dosyanın kaydedildiği CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar. |
| [GetRegion](./getregion/) | Çalışma kitabı için bölgesel ayarları alır veya ayarlar. |
| [SetRegion](./setregion/) | Çalışma kitabı için bölgesel ayarları alır veya ayarlar. |
| [GetGlobalizationSettings](./getglobalizationsettings/) | Küreselleştirme ayarlarını alır ve ayarlar. |
| [SetGlobalizationSettings](./setglobalizationsettings/) | Küreselleştirme ayarlarını alır ve ayarlar. |
| [GetNumberDecimalSeparator](./getnumberdecimalseparator/) | Sayısal değerlerin biçimlendirilmesi/çözülmesi için ondalık ayırıcıyı alır veya ayarlar. Varsayılan, geçerli Bölgenin ondalık ayırıcıdır. |
| [SetNumberDecimalSeparator](./setnumberdecimalseparator/) | Sayısal değerlerin biçimlendirilmesi/çözülmesi için ondalık ayırıcıyı alır veya ayarlar. Varsayılan, geçerli Bölgenin ondalık ayırıcıdır. |
| [GetNumberGroupSeparator](./getnumbergroupseparator/) | Sayısal değerlerde ondalık noktasının solundaki basamak gruplarını ayıran karakteri alır veya ayarlar. Varsayılan, geçerli Bölgenin grup ayırıcıdır. |
| [SetNumberGroupSeparator](./setnumbergroupseparator/) | Sayısal değerlerde ondalık noktasının solundaki basamak gruplarını ayıran karakteri alır veya ayarlar. Varsayılan, geçerli Bölgenin grup ayırıcıdır. |
| [GetPassword](./getpassword/) | Çalışma kitabı dosyası şifreleme parolasını temsil eder. |
| [SetPassword](./setpassword/) | Çalışma kitabı dosyası şifreleme parolasını temsil eder. |
| [GetWriteProtection](./getwriteprotection/) | Çalışma kitabının yazma koruma seçeneklerine erişim sağlar. |
| [IsEncrypted](./isencrypted/) | Bu çalışma kitabını açmak için bir şifrenin gerekli olup olmadığını gösteren bir değer alır. |
| [IsProtected](./isprotected/) | Çalışma kitabının yapısının veya penceresinin korumalı olup olmadığını gösteren bir değer alır. |
| [IsDefaultEncrypted](./isdefaultencrypted/) | Çalışma kitabının Yapısı ve Pencereleri kilitli olduğunda varsayılan şifreyle şifrelenip şifrelenmeyeceğini gösterir. |
| [SetIsDefaultEncrypted](./setisdefaultencrypted/) | Çalışma kitabının Yapısı ve Pencereleri kilitli olduğunda varsayılan şifreyle şifrelenip şifrelenmeyeceğini gösterir. |
| [IsMinimized](./isminimized/) | Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder. |
| [SetIsMinimized](./setisminimized/) | Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder. |
| [IsHidden](./ishidden/) | Bu çalışma kitabının gizli olup olmadığını gösterir. |
| [SetIsHidden](./setishidden/) | Bu çalışma kitabının gizli olup olmadığını gösterir. |
| [GetAutoCompressPictures](./getautocompresspictures/) | Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırıp sıkıştırmadığını gösteren bir Boolean değer belirler. |
| [SetAutoCompressPictures](./setautocompresspictures/) | Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırıp sıkıştırmadığını gösteren bir Boolean değer belirler. |
| [GetRemovePersonalInformation](./getremovepersonalinformation/) | Belirtilen çalışma kitabından kişisel bilgilerin kaldırılabileceği durumda doğru (True) döner. |
| [SetRemovePersonalInformation](./setremovepersonalinformation/) | Belirtilen çalışma kitabından kişisel bilgilerin kaldırılabileceği durumda doğru (True) döner. |
| [GetShapeDisplayType](./getshapedisplaytype/) | Uygulamanın bu çalışma kitabındaki şekilleri nasıl görüntülediğini alır ve ayarlar. |
| [SetShapeDisplayType](./setshapedisplaytype/) | Uygulamanın bu çalışma kitabındaki şekilleri nasıl görüntülediğini alır ve ayarlar. |
| [GetHidePivotFieldList](./gethidepivotfieldlist/) | PivotTable için alan listesinin gizlenip gizlenmeyeceğini alır ve ayarlar. |
| [SetHidePivotFieldList](./sethidepivotfieldlist/) | PivotTable için alan listesinin gizlenip gizlenmeyeceğini alır ve ayarlar. |
| [GetMaxUniqueItemsPerField](./getmaxuniqueitemsperfield/) | Alan başına benzersiz öğe sayısının sınırlamasını alır ve ayarlar. |
| [SetMaxUniqueItemsPerField](./setmaxuniqueitemsperfield/) | Alan başına benzersiz öğe sayısının sınırlamasını alır ve ayarlar. |
| [GetUpdateLinksType](./getupdatelinkstype/) | Çalışma kitabı açıldığında dış bağlantıların nasıl güncelleneceğini alır ve ayarlar. |
| [SetUpdateLinksType](./setupdatelinkstype/) | Çalışma kitabı açıldığında dış bağlantıların nasıl güncelleneceğini alır ve ayarlar. |
| [SetPageOrientationType](./setpageorientationtype/) | Tüm çalışma kitabı için yazdırma yönlendirme tipini ayarlar. |
| [GetMaxRow](./getmaxrow/) | Sıfır tabanlı maksimum satır indeksini alır. |
| [GetMaxColumn](./getmaxcolumn/) | Sıfır tabanlı maksimum sütun indeksini alır. |
| [GetSmartTagOptions](./getsmarttagoptions/) | Akıllı etiketin seçeneklerini alır. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Bu çalışma kitabı için stil ile ilgili özelliklerin varsayılan değer ayarlarını alır. |
| [GetWindowLeft](./getwindowleft/) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde. |
| [SetWindowLeft](./setwindowleft/) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde. |
| [GetWindowLeftInch](./getwindowleftinch/) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, inç biriminde. |
| [SetWindowLeftInch](./setwindowleftinch/) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, inç biriminde. |
| [GetWindowLeftCM](./getwindowleftcm/) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, santimetre biriminde. |
| [SetWindowLeftCM](./setwindowleftcm/) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, santimetre biriminde. |
| [GetWindowTop](./getwindowtop/) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, nokta biriminde. |
| [SetWindowTop](./setwindowtop/) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, nokta biriminde. |
| [GetWindowTopInch](./getwindowtopinch/) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, inç biriminde. |
| [SetWindowTopInch](./setwindowtopinch/) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, inç biriminde. |
| [GetWindowTopCM](./getwindowtopcm/) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, santimetre biriminde. |
| [SetWindowTopCM](./setwindowtopcm/) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, santimetre biriminde. |
| [GetWindowWidth](./getwindowwidth/) | Pencerenin genişliği, nokta biriminde. |
| [SetWindowWidth](./setwindowwidth/) | Pencerenin genişliği, nokta biriminde. |
| [GetWindowWidthInch](./getwindowwidthinch/) | Pencerenin genişliği, inç biriminde. |
| [SetWindowWidthInch](./setwindowwidthinch/) | Pencerenin genişliği, inç biriminde. |
| [GetWindowWidthCM](./getwindowwidthcm/) | Pencerenin genişliği, santimetre biriminde. |
| [SetWindowWidthCM](./setwindowwidthcm/) | Pencerenin genişliği, santimetre biriminde. |
| [GetWindowHeight](./getwindowheight/) | Pencerenin yüksekliği, nokta biriminde. |
| [SetWindowHeight](./setwindowheight/) | Pencerenin yüksekliği, nokta biriminde. |
| [GetWindowHeightInch](./getwindowheightinch/) | Pencerenin yüksekliği, inç biriminde. |
| [SetWindowHeightInch](./setwindowheightinch/) | Pencerenin yüksekliği, inç biriminde. |
| [GetWindowHeightCM](./getwindowheightcm/) | Pencerenin yüksekliği, santimetre biriminde. |
| [SetWindowHeightCM](./setwindowheightcm/) | Pencerenin yüksekliği, santimetre biriminde. |
| [GetUpdateAdjacentCellsBorder](./getupdateadjacentcellsborder/) | Komşu hücrelerin kenarlığının güncellenip güncellenmeyeceğini gösterir. |
| [SetUpdateAdjacentCellsBorder](./setupdateadjacentcellsborder/) | Komşu hücrelerin kenarlığının güncellenip güncellenmeyeceğini gösterir. |
| [GetSignificantDigitsType](./getsignificantdigitstype/) | Bu çalışma kitabında sayısal değerlerin çıktısı için anlamlı basamak türünü alır ve ayarlar. Varsayılan değer CellsHelper.SignificantDigitsType'tir. |
| [SetSignificantDigitsType](./setsignificantdigitstype/) | Bu çalışma kitabında sayısal değerlerin çıktısı için anlamlı basamak türünü alır ve ayarlar. Varsayılan değer CellsHelper.SignificantDigitsType'tir. |
| [GetCheckCompatibility](./getcheckcompatibility/) | Çalışma kitabı kaydedilirken daha eski sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir. |
| [SetCheckCompatibility](./setcheckcompatibility/) | Çalışma kitabı kaydedilirken daha eski sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir Exception alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen hatalar oluşabilir. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir Exception alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen hatalar oluşabilir. |
| [GetAutoRecover](./getautorecover/) | Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir. |
| [SetAutoRecover](./setautorecover/) | Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir. |
| [GetCrashSave](./getcrashsave/) | Uygulamanın bir çöküşten sonra çalışma kitabı dosyasını son olarak kaydedip kaydetmediğini gösterir. |
| [SetCrashSave](./setcrashsave/) | Uygulamanın bir çöküşten sonra çalışma kitabı dosyasını son olarak kaydedip kaydetmediğini gösterir. |
| [GetDataExtractLoad](./getdataextractload/) | Uygulamanın veri kurtarma için çalışma kitabını son olarak açıp açmadığını gösterir. |
| [SetDataExtractLoad](./setdataextractload/) | Uygulamanın veri kurtarma için çalışma kitabını son olarak açıp açmadığını gösterir. |
| [GetRepairLoad](./getrepairload/) | Uygulamanın çalışma kitabını son olarak güvenli ya da onarım modunda açıp açmadığını gösterir. |
| [SetRepairLoad](./setrepairload/) | Uygulamanın çalışma kitabını son olarak güvenli ya da onarım modunda açıp açmadığını gösterir. |
| [GetBuildVersion](./getbuildversion/) | Uygulamanın artımlı genel sürümünü belirtir. |
| [SetBuildVersion](./setbuildversion/) | Uygulamanın artımlı genel sürümünü belirtir. |
| [GetMemorySetting](./getmemorysetting/) | Bellek kullanım seçeneklerini alır veya ayarlar. Yeni seçenek yeni oluşturulan çalışma sayfaları için varsayılan seçenek olarak alınır ancak mevcut çalışma sayfaları için etkili olmaz. |
| [SetMemorySetting](./setmemorysetting/) | Bellek kullanım seçeneklerini alır veya ayarlar. Yeni seçenek yeni oluşturulan çalışma sayfaları için varsayılan seçenek olarak alınır ancak mevcut çalışma sayfaları için etkili olmaz. |
| [GetPaperSize](./getpapersize/) | Varsayılan yazdırma kağıt boyutunu alır ve ayarlar. |
| [SetPaperSize](./setpapersize/) | Varsayılan yazdırma kağıt boyutunu alır ve ayarlar. |
| [GetMaxRowsOfSharedFormula](./getmaxrowsofsharedformula/) | Paylaşımlı formülün maksimum satır sayısını alır ve ayarlar. |
| [SetMaxRowsOfSharedFormula](./setmaxrowsofsharedformula/) | Paylaşımlı formülün maksimum satır sayısını alır ve ayarlar. |
| [GetCompliance](./getcompliance/) | Çıktı belgesi için OOXML sürümünü belirtir. Varsayılan değer Ecma376_2006'dır. |
| [SetCompliance](./setcompliance/) | Çıktı belgesi için OOXML sürümünü belirtir. Varsayılan değer Ecma376_2006'dır. |
| [GetQuotePrefixToStyle](./getquoteprefixtostyle/) | Hücreye dize değeri (tek tırnak işaretiyle başlayan) girerken Style.QuotePrefix özelliğinin ayarlanıp ayarlanmadığını gösterir. |
| [SetQuotePrefixToStyle](./setquoteprefixtostyle/) | Hücreye dize değeri (tek tırnak işaretiyle başlayan) girerken Style.QuotePrefix özelliğinin ayarlanıp ayarlanmadığını gösterir. |
| [GetFormulaSettings](./getformulasettings/) | Formül ile ilgili özelliklerin ayarlarını alır. |
| [GetPropertiesFollowChartPoint](./getpropertiesfollowchartpoint/) | Bu çalışma kitabındaki tüm grafiklerdeki veri noktası özellikleri ve veri etiketlerinin referanslarını takip edip etmediğini gösterir. |
| [SetPropertiesFollowChartPoint](./setpropertiesfollowchartpoint/) | Bu çalışma kitabındaki tüm grafiklerdeki veri noktası özellikleri ve veri etiketlerinin referanslarını takip edip etmediğini gösterir. |
| [GetDiscardImageEditData](./getdiscardimageeditdata/) | Görüntü verisinin düzenlemesinin atılıp atılmadığını gösterir. |
| [SetDiscardImageEditData](./setdiscardimageeditdata/) | Görüntü verisinin düzenlemesinin atılıp atılmadığını gösterir. |
| [GetDefaultImageResolution](./getdefaultimageresolution/) | Görüntünün varsayılan çözünürlüğünü alır ve ayarlar. |
| [SetDefaultImageResolution](./setdefaultimageresolution/) | Görüntünün varsayılan çözünürlüğünü alır ve ayarlar. |
| [GetWpsCompatibility](./getwpscompatibility/) | WPS ile uyumlu olup olmayacağını gösterir. |
| [SetWpsCompatibility](./setwpscompatibility/) | WPS ile uyumlu olup olmayacağını gösterir. |
