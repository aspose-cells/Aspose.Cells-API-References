---
title: "WorkbookSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çalışma kitabının tüm ayarlarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Çalışma kitabının tüm ayarlarını temsil eder.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [dispose()](#dispose--) | Kaynakları serbest bırakır. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Dosyanın yazarını alır. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırdığını gösteren bir boolean değer belirler. |
| [getAutoRecover()](#getAutoRecover--) | Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir. |
| [getBuildVersion()](#getBuildVersion--) | Uygulamanın artımlı genel sürümünü belirler. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Çalışma kitabı kaydedilirken önceki sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini gösterir. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Çıktı belgesi için OOXML sürümünü belirler. |
| [getCrashSave()](#getCrashSave--) | Uygulamanın çöküşten sonra çalışma kitabı dosyasını en son kaydedip kaydetmediğini gösterir. |
| [getDataExtractLoad()](#getDataExtractLoad--) | Uygulamanın veri kurtarma için çalışma kitabını en son açıp açmadığını gösterir. |
| [getDate1904()](#getDate1904--) | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | Görselin varsayılan çözünürlüğünü alır. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Bu çalışma kitabı için stil ile ilgili özelliklerin varsayılan değer ayarlarını alır. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | Görsel verisinin düzenlemesinin atılıp atılmayacağını gösterir. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Çalışma kitabında nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini belirtir. |
| [getEnableMacros()](#getEnableMacros--) | Makroları etkinleştir; |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | İlk görünen çalışma sayfası sekmesini alır. |
| [getFormulaSettings()](#getFormulaSettings--) | Formül ile ilgili özelliklerin ayarlarını alır. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Küreselleştirme ayarlarını alır. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | PivotTable için alan listesinin gizlenip gizlenmediğini alır. |
| [getLanguageCode()](#getLanguageCode--) | Dosyayı kaydeden CountryCode temelinde Çalışma Kitabı sürümünün kullanıcı arayüzü dilini alır. |
| [getLocale()](#getLocale--) | Bu çalışma kitabı tarafından kullanılan yerel ayarı alır. |
| [getMaxColumn()](#getMaxColumn--) | Sıfır tabanlı maksimum sütun indeksini alır. |
| [getMaxRow()](#getMaxRow--) | Sıfır tabanlı maksimum satır indeksini alır. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | Paylaşılan formülün maksimum satır numarasını alır. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | Alana göre benzersiz öğelerin sınırlamasını alır |
| [getMemorySetting()](#getMemorySetting--) | Bellek kullanım seçeneklerini alır. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı alır. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | Sayısal değerlerde ondalık noktasının solundaki basamak gruplarını ayıran karakteri alır. |
| [getPaperSize()](#getPaperSize--) | Varsayılan yazdırma kağıt boyutunu alır. |
| [getPassword()](#getPassword--) | Workbook dosyası şifreleme parolasını temsil eder. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | Bu çalışma kitabındaki tüm grafiklerdeki veri noktası özelliklerinin ve veri etiketlerinin referanslarını takip edip etmediğini gösterir. |
| [getProtectionType()](#getProtectionType--) | Çalışma kitabının koruma türünü alır. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Hücreye tek tırnak işaretiyle başlayan bir dize değeri girildiğinde [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) özelliğinin ayarlanıp ayarlanmadığını gösterir. |
| [getRegion()](#getRegion--) | Çalışma kitabı için bölgesel ayarları alır. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | Belirtilen çalışma kitabından kişisel bilgilerin kaldırılabileceği durumda doğru. |
| [getRepairLoad()](#getRepairLoad--) | Uygulamanın çalışma kitabını en son güvenli ya da onarım modunda açıp açmadığını gösterir. |
| [getResourceProvider()](#getResourceProvider--) | Harici kaynak için akış sağlayıcısını alır, örneğin "LinkToFile" türündeki resim verisini yüklemek gibi. |
| [getShapeDisplayType()](#getShapeDisplayType--) | Uygulamanın bu çalışma kitabındaki şekilleri nasıl görüntülediğini alır. |
| [getShared()](#getShared--) | Workbook'un paylaşılıp paylaşılmadığını gösteren bir değeri alır. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'i cinsinden). |
| [getShowTabs()](#getShowTabs--) | Workbook sekmelerinin görüntülenip görüntülenmediğini gösteren bir değeri alır. |
| [getSignificantDigits()](#getSignificantDigits--) | Önemli basamak sayısını alır. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Bu çalışma kitabında sayısal değerleri çıkartmak için kullanılan anlamlı basamak türünü alır. |
| [getSmartTagOptions()](#getSmartTagOptions--) | Akıllı etiket seçeneklerini alır. |
| [getStreamProvider()](#getStreamProvider--) | Harici kaynak için akış sağlayıcısını alır. |
| [getThemeFont(int type)](#getThemeFont-int-) | Varsayılan tema yazı tipi adını alır. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Komşu hücrelerin kenarlığının güncellenip güncellenmediğini gösterir. |
| [getUpdateLinksType()](#getUpdateLinksType--) | Çalışma kitabı açıldığında harici bağlantıların nasıl güncellendiğini alır. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [getWindowHeight()](#getWindowHeight--) | Pencerenin yüksekliği, nokta biriminde. |
| [getWindowHeightCM()](#getWindowHeightCM--) | Pencerenin yüksekliği, santimetre biriminde. |
| [getWindowHeightInch()](#getWindowHeightInch--) | Pencerenin yüksekliği, inç biriminde. |
| [getWindowLeft()](#getWindowLeft--) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde. |
| [getWindowLeftCM()](#getWindowLeftCM--) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. |
| [getWindowLeftInch()](#getWindowLeftInch--) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. |
| [getWindowTop()](#getWindowTop--) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, nokta biriminde. |
| [getWindowTopCM()](#getWindowTopCM--) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, santimetre biriminde. |
| [getWindowTopInch()](#getWindowTopInch--) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, inç biriminde. |
| [getWindowWidth()](#getWindowWidth--) | Pencerenin genişliği, nokta biriminde. |
| [getWindowWidthCM()](#getWindowWidthCM--) | Pencerenin genişliği, santimetre biriminde. |
| [getWindowWidthInch()](#getWindowWidthInch--) | Pencerenin genişliği, inç biriminde. |
| [getWpsCompatibility()](#getWpsCompatibility--) | WPS ile uyumlu olup olmadığını gösterir. |
| [getWriteProtection()](#getWriteProtection--) | Çalışma kitabının yazma koruma seçeneklerine erişim sağlar. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Çalışma kitabının Yapısı ve Pencereleri kilitliyse, varsayılan şifreyle şifrelenip şifrelenmeyeceğini gösterir. |
| [isEncrypted()](#isEncrypted--) | Bu çalışma kitabını açmak için şifre gerekip gerekmediğini gösteren bir değer alır. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermeyeceğini gösteren bir değer alır. |
| [isHidden()](#isHidden--) | Bu çalışma kitabının gizli olup olmadığını gösterir. |
| [isMinimized()](#isMinimized--) | Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder. |
| [isProtected()](#isProtected--) | Çalışma kitabının yapısının veya penceresinin korumalı olup olmadığını gösteren bir değer alır. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermeyeceğini gösteren bir değer alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Dosyanın yazarını ayarlar. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırdığını gösteren bir boolean değer belirler. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | Uygulamanın artımlı genel sürümünü belirler. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | Çalışma kitabı kaydedilirken önceki sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini gösterir. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setCompliance(int value)](#setCompliance-int-) | Çıktı belgesi için OOXML sürümünü belirler. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | Uygulamanın çöküşten sonra çalışma kitabı dosyasını en son kaydedip kaydetmediğini gösterir. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | Uygulamanın veri kurtarma için çalışma kitabını en son açıp açmadığını gösterir. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri ayarlar. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | Çalışma kitabının Yapısı ve Pencereleri kilitliyse, varsayılan şifreyle şifrelenip şifrelenmeyeceğini gösterir. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | Görselin varsayılan çözünürlüğünü ayarlar. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | Görsel verisinin düzenlemesinin atılıp atılmayacağını gösterir. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | Çalışma kitabında nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini belirtir. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Makroları etkinleştir; |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | İlk görünür çalışma sayfası sekmesini ayarlar. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | Küreselleştirme ayarlarını ayarlar. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri ayarlar. |
| [setHidden(boolean value)](#setHidden-boolean-) | Bu çalışma kitabının gizli olup olmadığını gösterir. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | Özet Tablo için alan listesinin gizlenip gizlenmeyeceğini ayarlar. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Dosyayı kaydeden CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini ayarlar. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Bu çalışma kitabı tarafından kullanılan Locale'i ayarlar. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | Paylaşılan formülün maksimum satır sayısını ayarlar. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | Alan başına benzersiz öğe sınırlamasını ayarlar. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Bellek kullanım seçeneklerini ayarlar. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı ayarlar. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | Sayısal değerlerde ondalık noktasının solundaki basamak gruplarını ayıran karakteri ayarlar. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Tüm çalışma kitabı için baskı yönlendirme tipini ayarlar. |
| [setPaperSize(int value)](#setPaperSize-int-) | Varsayılan baskı kağıt boyutunu ayarlar. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Workbook dosyası şifreleme parolasını temsil eder. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | Bu çalışma kitabındaki tüm grafiklerdeki veri noktası özelliklerinin ve veri etiketlerinin referanslarını takip edip etmediğini gösterir. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | Hücreye tek tırnak işaretiyle başlayan bir dize değeri girildiğinde [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) özelliğinin ayarlanıp ayarlanmadığını gösterir. |
| [setRegion(int value)](#setRegion-int-) | Çalışma kitabı için bölgesel ayarları ayarlar. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | Belirtilen çalışma kitabından kişisel bilgilerin kaldırılabileceği durumda doğru. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | Uygulamanın çalışma kitabını en son güvenli ya da onarım modunda açıp açmadığını gösterir. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | Harici kaynak için akış sağlayıcısını ayarlar, örneğin "LinkToFile" türündeki resim verisini yüklemek gibi. |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | Uygulamanın bu çalışma kitabındaki şekilleri nasıl görüntüleyeceğini ayarlar. |
| [setShared(boolean value)](#setShared-boolean-) | Çalışma kitabının paylaşılıp paylaşılmadığını gösteren bir değeri ayarlar. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'i cinsinden). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | Çalışma kitabı sekmelerinin görüntülenip görüntülenmeyeceğini belirten bir değeri ayarlar. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Önemli basamak sayısını ayarlar. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Bu çalışma kitabında sayısal değerlerin çıktısı için anlamlı basamak tipini ayarlar. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Harici kaynak için akış sağlayıcısını ayarlar. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | Komşu hücrelerin kenarlığının güncellenip güncellenmediğini gösterir. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | Çalışma kitabı açıldığında harici bağlantıların nasıl güncelleneceğini ayarlar. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri ayarlar. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | Pencerenin yüksekliği, nokta biriminde. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | Pencerenin yüksekliği, santimetre biriminde. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | Pencerenin yüksekliği, inç biriminde. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. |
| [setWindowTop(double value)](#setWindowTop-double-) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, nokta biriminde. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, santimetre biriminde. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, inç biriminde. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | Pencerenin genişliği, nokta biriminde. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | Pencerenin genişliği, santimetre biriminde. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | Pencerenin genişliği, inç biriminde. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | WPS ile uyumlu olup olmadığını gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


Kaynakları serbest bırakır.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Dosyanın yazarını alır.

**Remarks**

Ayarlanmamış, önce [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) kontrol edin, ardından Environment kullanıcısını kontrol edin.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırdığını gösteren bir boolean değer belirler.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Uygulamanın artımlı genel sürümünü belirler.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Çalışma kitabı kaydedilirken önceki sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir.

**Remarks**

Varsayılan değer true'dur. Yalnızca Excel97-2003 xls veya xlt dosyaları için.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini gösterir.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi bir yöntemle 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Çıktı belgesi için OOXML sürümünü belirtir. Varsayılan değer Ecma376\_2006'dır.

Bakınız [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Yalnızca .xlsx dosyaları için.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


Uygulamanın çöküşten sonra çalışma kitabı dosyasını en son kaydedip kaydetmediğini gösterir.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


Uygulamanın veri kurtarma için çalışma kitabını en son açıp açmadığını gösterir.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


Görselin varsayılan çözünürlüğünü alır.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Bu çalışma kitabı için stil ile ilgili özelliklerin varsayılan değer ayarlarını alır.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


Görsel verisinin düzenlemesinin atılıp atılmayacağını gösterir.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Çalışma kitabında nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini belirtir.

Bakınız [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Makroları etkinleştir;

**Remarks**

Şimdi yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


İlk görünen çalışma sayfası sekmesini alır.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


Formül ile ilgili özelliklerin ayarlarını alır.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


Küreselleştirme ayarlarını alır.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


PivotTable için alan listesinin gizlenip gizlenmediğini alır.

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Dosyayı kaydeden CountryCode temelinde Çalışma Kitabı sürümünün kullanıcı arayüzü dilini alır.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Bu çalışma kitabı tarafından kullanılan yerel ayarı alır.

**Remarks**

Locale ve [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) ikisi de ayarlanmamışsa null döndürür.

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Sıfır tabanlı maksimum sütun indeksini alır.

**Remarks**

Dosya formatı Excel97-2003 ise 255 döndürür;

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Sıfır tabanlı maksimum satır indeksini alır.

**Remarks**

Dosya formatı Excel97-2003 ise 65535 döndürür;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


Paylaşılan formülün maksimum satır numarasını alır.

**Remarks**

Sayı çok büyükse, otomatik filtre MS Excel 2013'te çok yavaş çalışır.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


Alana göre benzersiz öğelerin sınırlamasını alır

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Bellek kullanımı seçeneklerini alır. Yeni seçenek yeni oluşturulan çalışma sayfaları için varsayılan seçenek olarak alınır ancak mevcut çalışma sayfaları için etkili olmaz.

Bakınız [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Bellek modu hakkında daha fazla ayrıntı için lütfen [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--) adresine bakın.

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı alır. Varsayılan, geçerli Bölgenin ondalık ayırıcısıdır.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


Sayısal değerlerde ondalıktan sol taraftaki basamak gruplarını ayıran karakteri alır. Varsayılan, geçerli Bölgenin grup ayırıcıdır.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Varsayılan yazdırma kağıt boyutunu alır.

Bakınız [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Kağıt boyutu ile ilgili bir ayar yoksa, MS Excel varsayılan yazıcı ayarını kullanacaktır.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


Workbook dosyası şifreleme parolasını temsil eder.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


Bu çalışma kitabındaki tüm grafiklerdeki veri noktası özelliklerinin ve veri etiketlerinin referanslarını takip edip etmediğini gösterir.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Çalışma kitabının koruma türünü alır.

Bakınız [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Hücreye tek tırnak işaretiyle başlayan bir dize değeri girildiğinde [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) özelliğinin ayarlanıp ayarlanmadığını gösterir.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Çalışma kitabı için bölgesel ayarları alır.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Şablon dosyasından yüklenen bir çalışma kitabı için Aspose.Cells bileşeni tarafından kullanılan bölgesel ayarlar: i). XLS dosyası için bölgesel ayarlar için tanımlı alanlar vardır ve MS Excel, XLS dosyasını kaydederken bölgesel ayar verilerini dosyaya kaydeder. Bu nedenle, çalışma kitabı için şablon dosyasındaki kaydedilmiş bölgeyi kullanırız. XLS dosyasında kaydedilen bölgeyi kullanmak istemiyorsanız, şablon dosyasını yükledikten sonra (örneğin CountryCode.Default gibi) beklenen bölgeye sıfırlayın. Ayrıca, bu yöntemle belirttiğiniz kullanıcı değerini bir XLS dosyası kaydederken dosyaya da kaydederiz. ii). XLSX, XLSB... gibi diğer dosya formatları için dosya formatı spesifikasyonunda bölgesel ayarlar için tanımlı bir alan yoktur. Bu yüzden, çalışma kitabı için uygulamanın ortamının bölgesel ayarlarını kullanırız. Ve, bu yöntemle belirtilen kullanıcı değeri, bu dosya formatlarıyla oluşturulan dosyalarda tutulamaz. 2. MS Excel'de görüntüleme etkisi için: Burada uygulanan bölgesel ayarlar yalnızca Aspose.Cells bileşeniyle çalışma zamanında etkili olur ve MS Excel ile oluşturulan dosya görüntülenirken etkili olmaz. Belirtilen bölgesel ayar verileri kaydedilmiş olsa bile, oluşturulan XLS dosyası MS Excel ile görüntülendiğinde/düzenlendiğinde, MS Excel'in biçimlendirme için kullandığı bölge her zaman MS Excel'in çalıştığı ortamın varsayılan bölgesel ayarlarıdır, dosyada kaydedilen değil. Bu, MS Excel'in davranışıdır ve kodla değiştirilemez.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


Belirtilen çalışma kitabından kişisel bilgilerin kaldırılabileceği durumda doğru.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


Uygulamanın çalışma kitabını en son güvenli ya da onarım modunda açıp açmadığını gösterir.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


Harici kaynak için akış sağlayıcısını alır, örneğin "LinkToFile" türündeki resim verisini yüklemek gibi.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


Uygulamanın bu çalışma kitabındaki şekilleri nasıl görüntülediğini alır.

Bakınız [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


Workbook'un paylaşılıp paylaşılmadığını gösteren bir değeri alır.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'i cinsinden).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


Workbook sekmelerinin görüntülenip görüntülenmediğini gösteren bir değeri alır.

**Remarks**

Varsayılan değer true'tır.

**Example**

Aşağıdaki kod, elektronik tablonun Sayfa Sekmelerini ve Sekme Kaydırma Düğmelerini gizler.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


Önemli basamak sayısını alır. Varsayılan değer [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--) 'dır.

**Remarks**

Şu anda yalnızca 15 veya 17 olabilir. NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--) kullanın. Bu özellik, Haziran 2025'ten itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


Bu çalışma kitabında sayısal değerlerin çıktısı için önemli basamak tipini alır. Varsayılan değer [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--) 'dır.

Bakınız [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


Akıllı etiket seçeneklerini alır.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Harici kaynak için akış sağlayıcısını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ResourceProvider özelliğini kullanın. Bu özellik, Haziran 2022'den itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


Varsayılan tema yazı tipi adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). Yazı tipinin şema türü. |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Komşu hücrelerin kenarlığının güncellenip güncellenmediğini gösterir.

**Remarks**

Varsayılan değer false'tur. Örneğin: A1 hücresinin alt kenarı güncellenirse, A2 hücresinin üst kenarı da değişmelidir.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


Çalışma kitabı açıldığında harici bağlantıların nasıl güncellendiğini alır.

Bakınız [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Uyarı geri çağrısını alır.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


Pencerenin yüksekliği, nokta biriminde.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


Pencerenin yüksekliği, santimetre biriminde.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


Pencerenin yüksekliği, inç biriminde.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. Birimi santimetredir.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. Birimi inçtir.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, nokta biriminde.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, santimetre biriminde.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, inç biriminde.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


Pencerenin genişliği, nokta biriminde.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


Pencerenin genişliği, santimetre biriminde.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


Pencerenin genişliği, inç biriminde.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


WPS ile uyumlu olup olmadığını gösterir.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


Çalışma kitabının yazma koruma seçeneklerine erişim sağlar.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


Çalışma kitabının Yapısı ve Pencereleri kilitliyse, varsayılan şifreyle şifrelenip şifrelenmeyeceğini gösterir.

**Remarks**

Varsayılan değer şu anda false'tur. MS Excel 2013 ile aynıdır.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Bu çalışma kitabını açmak için şifre gerekip gerekmediğini gösteren bir değer alır.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermeyeceğini gösteren bir değer alır.

**Remarks**

Varsayılan değer true'tır.

**Example**

Aşağıdaki kod, elektronik tablo için yatay kaydırma çubuğunu görünmez yapar.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Bu çalışma kitabının gizli olup olmadığını gösterir.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Çalışma kitabının yapısının veya penceresinin korumalı olup olmadığını gösteren bir değer alır.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermeyeceğini gösteren bir değer alır.

**Remarks**

Varsayılan değer true'tır.

**Example**

Aşağıdaki kod, elektronik tablo için dikey kaydırma çubuğunu görünmez yapar.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Dosyanın yazarını ayarlar.

**Remarks**

Ayarlanmamış, önce [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) kontrol edin, ardından Environment kullanıcısını kontrol edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


Uygulamanın çalışma kitabındaki resimleri otomatik olarak sıkıştırdığını gösteren bir boolean değer belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


Uygulamanın artımlı genel sürümünü belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


Çalışma kitabı kaydedilirken önceki sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir.

**Remarks**

Varsayılan değer true'dur. Yalnızca Excel97-2003 xls veya xlt dosyaları için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi bir yöntemle 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Çıktı belgesi için OOXML sürümünü belirtir. Varsayılan değer Ecma376\_2006'dır.

Bakınız [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Yalnızca .xlsx dosyaları için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


Uygulamanın çöküşten sonra çalışma kitabı dosyasını en son kaydedip kaydetmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


Uygulamanın veri kurtarma için çalışma kitabını en son açıp açmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


Çalışma kitabının Yapısı ve Pencereleri kilitliyse, varsayılan şifreyle şifrelenip şifrelenmeyeceğini gösterir.

**Remarks**

Varsayılan değer şu anda false'tur. MS Excel 2013 ile aynıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


Görselin varsayılan çözünürlüğünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


Görsel verisinin düzenlemesinin atılıp atılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


Çalışma kitabında nesnelerin gösterilip gösterilmeyeceğini ve nasıl gösterileceğini belirtir.

Bakınız [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Makroları etkinleştir;

**Remarks**

Şimdi yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


İlk görünür çalışma sayfası sekmesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


Küreselleştirme ayarlarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


Oluşturulan elektronik tablonun yatay kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri ayarlar.

**Remarks**

Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Bu çalışma kitabının gizli olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


Özet Tablo için alan listesinin gizlenip gizlenmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Dosyayı kaydeden CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini ayarlar.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Bu çalışma kitabı tarafından kullanılan Locale'i ayarlar.

**Remarks**

Locale ve [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) ikisi de ayarlanmamışsa null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


Paylaşılan formülün maksimum satır sayısını ayarlar.

**Remarks**

Sayı çok büyükse, otomatik filtre MS Excel 2013'te çok yavaş çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


Alan başına benzersiz öğe sınırlamasını ayarlar.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Bellek kullanım seçeneklerini ayarlar. Yeni seçenek, yeni oluşturulan çalışma sayfaları için varsayılan seçenek olarak alınacak, ancak mevcut çalışma sayfaları için etkili olmayacaktır.

Bakınız [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Bellek modu hakkında daha fazla ayrıntı için lütfen [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--) adresine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı ayarlar. Varsayılan, geçerli Bölgenin ondalık ayırıcısıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


Sayısal değerlerde ondalık noktasının solundaki basamak gruplarını ayıran karakteri ayarlar. Varsayılan, geçerli Bölgenin grup ayırıcıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


Tüm çalışma kitabı için baskı yönlendirme tipini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). Sayfa yönlendirme türü |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Varsayılan baskı kağıt boyutunu ayarlar.

Bakınız [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Kağıt boyutu ile ilgili bir ayar yoksa, MS Excel varsayılan yazıcı ayarını kullanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Workbook dosyası şifreleme parolasını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


Bu çalışma kitabındaki tüm grafiklerdeki veri noktası özelliklerinin ve veri etiketlerinin referanslarını takip edip etmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


Hücreye tek tırnak işaretiyle başlayan bir dize değeri girildiğinde [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) özelliğinin ayarlanıp ayarlanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Çalışma kitabı için bölgesel ayarları ayarlar.

Bakınız [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Şablon dosyasından yüklenen bir çalışma kitabı için Aspose.Cells bileşeni tarafından kullanılan bölgesel ayarlar: i). XLS dosyası için bölgesel ayarlar için tanımlı alanlar vardır ve MS Excel, XLS dosyasını kaydederken bölgesel ayar verilerini dosyaya kaydeder. Bu nedenle, çalışma kitabı için şablon dosyasındaki kaydedilmiş bölgeyi kullanırız. XLS dosyasında kaydedilen bölgeyi kullanmak istemiyorsanız, şablon dosyasını yükledikten sonra (örneğin CountryCode.Default gibi) beklenen bölgeye sıfırlayın. Ayrıca, bu yöntemle belirttiğiniz kullanıcı değerini bir XLS dosyası kaydederken dosyaya da kaydederiz. ii). XLSX, XLSB... gibi diğer dosya formatları için dosya formatı spesifikasyonunda bölgesel ayarlar için tanımlı bir alan yoktur. Bu yüzden, çalışma kitabı için uygulamanın ortamının bölgesel ayarlarını kullanırız. Ve, bu yöntemle belirtilen kullanıcı değeri, bu dosya formatlarıyla oluşturulan dosyalarda tutulamaz. 2. MS Excel'de görüntüleme etkisi için: Burada uygulanan bölgesel ayarlar yalnızca Aspose.Cells bileşeniyle çalışma zamanında etkili olur ve MS Excel ile oluşturulan dosya görüntülenirken etkili olmaz. Belirtilen bölgesel ayar verileri kaydedilmiş olsa bile, oluşturulan XLS dosyası MS Excel ile görüntülendiğinde/düzenlendiğinde, MS Excel'in biçimlendirme için kullandığı bölge her zaman MS Excel'in çalıştığı ortamın varsayılan bölgesel ayarlarıdır, dosyada kaydedilen değil. Bu, MS Excel'in davranışıdır ve kodla değiştirilemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


Belirtilen çalışma kitabından kişisel bilgilerin kaldırılabileceği durumda doğru.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


Uygulamanın çalışma kitabını en son güvenli ya da onarım modunda açıp açmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


Harici kaynak için akış sağlayıcısını ayarlar, örneğin "LinkToFile" türündeki resim verisini yüklemek gibi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


Uygulamanın bu çalışma kitabındaki şekilleri nasıl görüntüleyeceğini ayarlar.

Bakınız [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


Çalışma kitabının paylaşılıp paylaşılmadığını gösteren bir değeri ayarlar.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'i cinsinden).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


Çalışma kitabı sekmelerinin görüntülenip görüntülenmeyeceğini belirten bir değeri ayarlar.

**Remarks**

Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


Önemli basamak sayısını ayarlar. Varsayılan değer [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Şu anda yalnızca 15 veya 17 olabilir. NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--) kullanın. Bu özellik, Haziran 2025'ten itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


Bu çalışma kitabında sayısal değerlerin çıktısı için önemli basamak türünü ayarlar. Varsayılan değer [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Bakınız [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Harici kaynak için akış sağlayıcısını ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ResourceProvider özelliğini kullanın. Bu özellik, Haziran 2022'den itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


Komşu hücrelerin kenarlığının güncellenip güncellenmediğini gösterir.

**Remarks**

Varsayılan değer false'tur. Örneğin: A1 hücresinin alt kenarı güncellenirse, A2 hücresinin üst kenarı da değişmelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


Çalışma kitabı açıldığında harici bağlantıların nasıl güncelleneceğini ayarlar.

Bakınız [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


Oluşturulan elektronik tablonun dikey kaydırma çubuğu içerip içermeyeceğini gösteren bir değeri ayarlar.

**Remarks**

Varsayılan değer true'tır.

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

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


Pencerenin yüksekliği, nokta biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


Pencerenin yüksekliği, santimetre biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


Pencerenin yüksekliği, inç biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. Birimi santimetredir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. Birimi inçtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, nokta biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, santimetre biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, inç biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


Pencerenin genişliği, nokta biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


Pencerenin genişliği, santimetre biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


Pencerenin genişliği, inç biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


WPS ile uyumlu olup olmadığını gösterir.

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

