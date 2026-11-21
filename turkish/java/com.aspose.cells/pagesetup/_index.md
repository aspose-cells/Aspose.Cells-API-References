---
title: "PageSetup"
second_title: "Aspose.Cells for Java API Referansı"
description: "Sayfa ayarı açıklamasını temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

Sayfa ayarı açıklamasını temsil eden nesneyi kapsüller. PageSetup nesnesi tüm sayfa ayarı seçeneklerini içerir.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
         Worksheet sheet = sheets.get(1);
         PageSetup pageSetup = sheet.getPageSetup();
         pageSetup.setPrintArea("D1:K13");
 
         //do your business
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | Üstbilgi ve altbilgi ayarlarını temizler. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | Sayfa ayarının ayarını kopyalar. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | Özel kağıt boyutunu inç cinsinden ayarlar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | Belge öğelerinin siyah beyaz basılıp basılmayacağını temsil eder. |
| [getBottomMargin()](#getBottomMargin--) | Alt kenar boşluğunun boyutunu santimetre cinsinden temsil eder. |
| [getBottomMarginInch()](#getBottomMarginInch--) | Alt kenar boşluğunun boyutunu inç cinsinden temsil eder. |
| [getCenterHorizontally()](#getCenterHorizontally--) | Sayfanın yatay olarak ortalanıp ortalanmayacağını temsil eder. |
| [getCenterVertically()](#getCenterVertically--) | Sayfanın dikey olarak ortalanıp ortalanmayacağını temsil eder. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | Üst bilgi veya alt bilgi için tüm komutları alır. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | Excel dosyasının çift sayfa alt bilgisini biçimlendiren bir betik alır. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | Excel dosyasının çift sayfa üst bilgisini biçimlendiren bir betik alır. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | Excel dosyasının birinci sayfa alt bilgisini biçimlendiren bir betik alır. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | Excel dosyasının birinci sayfa üst bilgisini biçimlendiren bir betik alır. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Bu sayfa yazdırıldığında kullanılacak birinci sayfa numarasını temsil eder. |
| [getFitToPagesTall()](#getFitToPagesTall--) | Yazdırıldığında çalışma sayfasının kaç sayfa yüksekliğine ölçekleneceğini temsil eder. |
| [getFitToPagesWide()](#getFitToPagesWide--) | Yazdırıldığında çalışma sayfasının kaç sayfa genişliğine ölçekleneceğini temsil eder. |
| [getFooter(int section)](#getFooter-int-) | Excel dosyasının alt bilgisini biçimlendiren bir betik alır. |
| [getFooterMargin()](#getFooterMargin--) | Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi santimetre biriminde temsil eder. |
| [getFooterMarginInch()](#getFooterMarginInch--) | Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi inç biriminde temsil eder. |
| [getHeader(int section)](#getHeader-int-) | Excel dosyasının üst bilgisini biçimlendiren bir betik alır. |
| [getHeaderMargin()](#getHeaderMargin--) | Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi santimetre biriminde temsil eder. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi inç biriminde temsil eder. |
| [getLeftMargin()](#getLeftMargin--) | Sol kenar boşluğunun boyutunu santimetre biriminde temsil eder. |
| [getLeftMarginInch()](#getLeftMarginInch--) | Sol kenar boşluğunun boyutunu inç biriminde temsil eder. |
| [getODSPageBackground()](#getODSPageBackground--) | ODS'nin arka planını alır. |
| [getOrder()](#getOrder--) | Microsoft Excel'in büyük bir çalışma sayfasını yazdırırken sayfaları numaralandırmak için kullandığı sıralamayı temsil eder. |
| [getOrientation()](#getOrientation--) | Sayfa yazdırma yönünü temsil eder. |
| [getPaperHeight()](#getPaperHeight--) | Sayfa yönü dikkate alınarak kağıdın yüksekliğini inç biriminde alır. |
| [getPaperSize()](#getPaperSize--) | Kağıdın boyutunu temsil eder. |
| [getPaperWidth()](#getPaperWidth--) | Sayfa yönü dikkate alınarak kağıdın genişliğini inç biriminde alır. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | Üst bilgi / alt bilginin [Picture](../../com.aspose.cells/picture) nesnesini alır. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | Üst bilgi / alt bilginin [Picture](../../com.aspose.cells/picture) nesnesini alır. |
| [getPrintArea()](#getPrintArea--) | Yazdırılacak aralığı temsil eder. |
| [getPrintComments()](#getPrintComments--) | Yorumların sayfa ile birlikte nasıl yazdırıldığını temsil eder. |
| [getPrintCopies()](#getPrintCopies--) | Yazdırılacak kopya sayısını alır. |
| [getPrintDraft()](#getPrintDraft--) | Sayfanın grafik olmadan yazdırılıp yazdırılmayacağını temsil eder. |
| [getPrintErrors()](#getPrintErrors--) | Görüntülenen yazdırma hatası türünü belirtir. |
| [getPrintGridlines()](#getPrintGridlines--) | Hücre ızgara çizgilerinin sayfada yazdırılıp yazdırılmayacağını temsil eder. |
| [getPrintHeadings()](#getPrintHeadings--) | Satır ve sütun başlıklarının bu sayfada yazdırılıp yazdırılmayacağını temsil eder. |
| [getPrintQuality()](#getPrintQuality--) | Yazdırma kalitesini temsil eder. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | Her sayfanın sol tarafında tekrarlanacak hücreleri içeren sütunları temsil eder. |
| [getPrintTitleRows()](#getPrintTitleRows--) | Her sayfanın üst kısmında tekrarlanacak hücreleri içeren satırları temsil eder. |
| [getPrinterSettings()](#getPrinterSettings--) | Varsayılan yazıcının ayarlarını alır. |
| [getRightMargin()](#getRightMargin--) | Sağ kenar boşluğunun boyutunu, santimetre biriminde temsil eder. |
| [getRightMarginInch()](#getRightMarginInch--) | Sağ kenar boşluğunun boyutunu, inç biriminde temsil eder. |
| [getTopMargin()](#getTopMargin--) | Üst kenar boşluğunun boyutunu, santimetre biriminde temsil eder. |
| [getTopMarginInch()](#getTopMarginInch--) | Üst kenar boşluğunun boyutunu, inç biriminde temsil eder. |
| [getZoom()](#getZoom--) | Yüzde olarak ölçekleme faktörünü temsil eder. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | İlk sayfa numarasının otomatik olarak atanıp atanmadığını gösterir. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | Kağıt boyutunun otomatik olup olmadığını gösterir. |
| [isHFAlignMargins()](#isHFAlignMargins--) | Üst bilgi ve alt bilgi kenar boşluklarının sayfa kenar boşluklarıyla hizalanıp hizalanmadığını gösterir. |
| [isHFDiffFirst()](#isHFDiffFirst--) | Doğru, ilk sayfanın üst bilgi/alt bilgisinin diğer sayfalardan farklı olduğunu ifade eder. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | Doğru, tek sayfaların üst bilgi/alt bilgisinin diğer tek sayfalardan farklı olduğunu ifade eder. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | Üst bilgi ve alt bilginin belge ölçeklemesiyle ölçeklenip ölçeklenmediğini gösterir. |
| [isPercentScale()](#isPercentScale--) | Bu özellik False ise, FitToPagesWide ve FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol eder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | İlk sayfa numarasının otomatik olarak atanıp atanmadığını gösterir. |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | Belge öğelerinin siyah beyaz basılıp basılmayacağını temsil eder. |
| [setBottomMargin(double value)](#setBottomMargin-double-) | Alt kenar boşluğunun boyutunu santimetre cinsinden temsil eder. |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | Alt kenar boşluğunun boyutunu inç cinsinden temsil eder. |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | Sayfanın yatay olarak ortalanıp ortalanmayacağını temsil eder. |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | Sayfanın dikey olarak ortalanıp ortalanmayacağını temsil eder. |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | Bir Excel dosyasının çift sayfa alt bilgisini biçimlendiren bir betik ayarlar. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | Bir Excel dosyasının çift sayfa üst bilgisini biçimlendiren bir betik ayarlar. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | Bir Excel dosyasının ilk sayfa alt bilgisini biçimlendiren bir betik ayarlar. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | Bir Excel dosyasının ilk sayfa üst bilgisini biçimlendiren bir betik ayarlar. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | Bu sayfa yazdırıldığında kullanılacak birinci sayfa numarasını temsil eder. |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | Çalışma sayfasının yazdırıldığında ölçekleneceği sayfa sayısını ayarlar. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | Yazdırıldığında çalışma sayfasının kaç sayfa yüksekliğine ölçekleneceğini temsil eder. |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | Yazdırıldığında çalışma sayfasının kaç sayfa genişliğine ölçekleneceğini temsil eder. |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | Excel dosyasının altbilgisini biçimlendiren bir betik ayarlar. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi santimetre biriminde temsil eder. |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi inç biriminde temsil eder. |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | Bir çalışma sayfasının altbilgisine bir resim ayarlar. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | Üst bilgi ve alt bilgi kenar boşluklarının sayfa kenar boşluklarıyla hizalanıp hizalanmadığını gösterir. |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | Doğru, ilk sayfanın üst bilgi/alt bilgisinin diğer sayfalardan farklı olduğunu ifade eder. |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | Doğru, tek sayfaların üst bilgi/alt bilgisinin diğer tek sayfalardan farklı olduğunu ifade eder. |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | Üst bilgi ve alt bilginin belge ölçeklemesiyle ölçeklenip ölçeklenmediğini gösterir. |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | Excel dosyasının üstbilgisini biçimlendiren bir betik ayarlar. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi santimetre biriminde temsil eder. |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi inç biriminde temsil eder. |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | Bir çalışma sayfasının üstbilgisine bir resim ayarlar. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Sol kenar boşluğunun boyutunu santimetre biriminde temsil eder. |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | Sol kenar boşluğunun boyutunu inç biriminde temsil eder. |
| [setOrder(int value)](#setOrder-int-) | Microsoft Excel'in büyük bir çalışma sayfasını yazdırırken sayfaları numaralandırmak için kullandığı sıralamayı temsil eder. |
| [setOrientation(int value)](#setOrientation-int-) | Sayfa yazdırma yönünü temsil eder. |
| [setPaperSize(int value)](#setPaperSize-int-) | Kağıdın boyutunu temsil eder. |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | Bu özellik False ise, FitToPagesWide ve FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol eder. |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | Bir çalışma sayfasının üstbilgi/altbilgisine bir resim ayarlar. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | Yazdırılacak aralığı temsil eder. |
| [setPrintComments(int value)](#setPrintComments-int-) | Yorumların sayfa ile birlikte nasıl yazdırıldığını temsil eder. |
| [setPrintCopies(int value)](#setPrintCopies-int-) | Yazdırılacak kopya sayısını ayarlar. |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | Sayfanın grafik olmadan yazdırılıp yazdırılmayacağını temsil eder. |
| [setPrintErrors(int value)](#setPrintErrors-int-) | Görüntülenen yazdırma hatası türünü belirtir. |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | Hücre ızgara çizgilerinin sayfada yazdırılıp yazdırılmayacağını temsil eder. |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | Satır ve sütun başlıklarının bu sayfada yazdırılıp yazdırılmayacağını temsil eder. |
| [setPrintQuality(int value)](#setPrintQuality-int-) | Yazdırma kalitesini temsil eder. |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | Her sayfanın sol tarafında tekrarlanacak hücreleri içeren sütunları temsil eder. |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | Her sayfanın üst kısmında tekrarlanacak hücreleri içeren satırları temsil eder. |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | Varsayılan yazıcının ayarlarını ayarlar. |
| [setRightMargin(double value)](#setRightMargin-double-) | Sağ kenar boşluğunun boyutunu, santimetre biriminde temsil eder. |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | Sağ kenar boşluğunun boyutunu, inç biriminde temsil eder. |
| [setTopMargin(double value)](#setTopMargin-double-) | Üst kenar boşluğunun boyutunu, santimetre biriminde temsil eder. |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | Üst kenar boşluğunun boyutunu, inç biriminde temsil eder. |
| [setZoom(int value)](#setZoom-int-) | Yüzde olarak ölçekleme faktörünü temsil eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


Üstbilgi ve altbilgi ayarlarını temizler.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


Sayfa ayarının ayarını kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | Kaynak. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Kopyalama seçenekleri. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


Özel kağıt boyutunu inç cinsinden ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| genişlik | double | Kağıdın genişliği. |
| yükseklik | double | Kağıdın yüksekliği. |

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
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


Belge öğelerinin siyah beyaz basılıp basılmayacağını temsil eder.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


Alt kenar boşluğunun boyutunu santimetre cinsinden temsil eder.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


Alt kenar boşluğunun boyutunu inç cinsinden temsil eder.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


Sayfanın yatay olarak ortalanıp ortalanmayacağını temsil eder.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


Sayfanın dikey olarak ortalanıp ortalanmayacağını temsil eder.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommands(String headerFooterScript) {#getCommands-java.lang.String-}
```
public HeaderFooterCommand[] getCommands(String headerFooterScript)
```


Üst bilgi veya alt bilgi için tüm komutları alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| headerFooterScript | java.lang.String | Üstbilgi/altbilgi betiği |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - Üstbilgi veya altbilgi için tüm komutları döndürür.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


Excel dosyasının çift sayfa alt bilgisini biçimlendiren bir betik alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


Excel dosyasının çift sayfa üst bilgisini biçimlendiren bir betik alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


Excel dosyasının birinci sayfa alt bilgisini biçimlendiren bir betik alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


Excel dosyasının birinci sayfa üst bilgisini biçimlendiren bir betik alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


Bu sayfa yazdırıldığında kullanılacak birinci sayfa numarasını temsil eder.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


Çalışma sayfasının yazdırıldığında kaç sayfa yüksekliğine ölçekleneceğini temsil eder. Varsayılan değer 1'dir.

**Remarks**

Tüm satırları tek bir sayfaya sığdırmak istiyorsanız FitToPagesWide'ı sıfır olarak ayarlamanız gerekir.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


Çalışma sayfasının yazdırıldığında kaç sayfa genişliğine ölçekleneceğini temsil eder. Varsayılan değer 1'dir.

**Remarks**

Tüm sütunları tek bir sayfaya sığdırmak istiyorsanız FitToPagesTall'ı sıfır olarak ayarlamanız gerekir.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


Excel dosyasının alt bilgisini biçimlendiren bir betik alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi santimetre biriminde temsil eder.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi inç biriminde temsil eder.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


Excel dosyasının üst bilgisini biçimlendiren bir betik alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi santimetre biriminde temsil eder.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi inç biriminde temsil eder.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Sol kenar boşluğunun boyutunu santimetre biriminde temsil eder.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


Sol kenar boşluğunun boyutunu inç biriminde temsil eder.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


ODS'nin arka planını alır.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


Microsoft Excel'in büyük bir çalışma sayfasını yazdırırken sayfaları numaralandırmak için kullandığı sıralamayı temsil eder.

Bkz. [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Sayfa yazdırma yönünü temsil eder.

Bak [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


Sayfa yönü dikkate alınarak kağıdın yüksekliğini inç biriminde alır.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Kağıdın boyutunu temsil eder.

Bakınız [PaperSizeType](../../com.aspose.cells/papersizetype).

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


Sayfa yönü dikkate alınarak kağıdın genişliğini inç biriminde alır.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


Üst bilgi / alt bilginin [Picture](../../com.aspose.cells/picture) nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isFirst | boolean | İlk sayfa üstbilgi/altbilgi resmini alıp almayacağını gösterir. |
| isEven | boolean | Çift sayfa üstbilgi/altbilgi resmini alıp almayacağını gösterir. |
| isHeader | boolean | Üstbilgi/altbilgi resminin alınıp alınmadığını gösterir. |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


Üst bilgi / alt bilginin [Picture](../../com.aspose.cells/picture) nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isHeader | boolean | Üstbilgi veya altbilgide olup olmadığını gösterir. |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


Yazdırılacak aralığı temsil eder.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


Yorumların sayfa ile birlikte nasıl yazdırıldığını temsil eder.

Bakınız [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


Yazdırılacak kopya sayısını alır.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


Sayfanın grafik olmadan yazdırılıp yazdırılmayacağını temsil eder.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


Görüntülenen yazdırma hatası türünü belirtir.

Bak [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


Hücre ızgara çizgilerinin sayfada yazdırılıp yazdırılmayacağını temsil eder.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


Satır ve sütun başlıklarının bu sayfada yazdırılıp yazdırılmayacağını temsil eder.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


Yazdırma kalitesini temsil eder.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


Her sayfanın sol tarafında tekrarlanacak hücreleri içeren sütunları temsil eder.

**Example**

```
         pageSetup.setPrintTitleColumns("$A:$A");
```

**Returns:**
java.lang.String
### getPrintTitleRows() {#getPrintTitleRows--}
```
public String getPrintTitleRows()
```


Her sayfanın üst kısmında tekrarlanacak hücreleri içeren satırları temsil eder.

**Example**

```
         pageSetup.setPrintTitleRows("$1:$1");
```

**Returns:**
java.lang.String
### getPrinterSettings() {#getPrinterSettings--}
```
public byte[] getPrinterSettings()
```


Varsayılan yazıcının ayarlarını alır.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Sağ kenar boşluğunun boyutunu, santimetre biriminde temsil eder.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


Sağ kenar boşluğunun boyutunu, inç biriminde temsil eder.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


Üst kenar boşluğunun boyutunu, santimetre biriminde temsil eder.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


Üst kenar boşluğunun boyutunu, inç biriminde temsil eder.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


Yüzde olarak ölçek faktörünü temsil eder. 10 ile 400 arasında olmalıdır.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}
```
public boolean isAutoFirstPageNumber()
```


İlk sayfa numarasının otomatik olarak atanıp atanmadığını gösterir.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


Kağıt boyutunun otomatik olup olmadığını gösterir.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


Üstbilgi ve altbilgi kenar boşluklarının sayfa kenar boşluklarıyla hizalanıp hizalanmadığını gösterir. Bu özellik true ise, sol üstbilgi ve altbilgi sol kenar boşluğuyla, sağ üstbilgi ve altbilgi sağ kenar boşluğuyla hizalanır. Bu seçenek varsayılan olarak etkindir.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


Doğru, ilk sayfanın üst bilgi/alt bilgisinin diğer sayfalardan farklı olduğunu ifade eder.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


Doğru, tek sayfaların üst bilgi/alt bilgisinin diğer tek sayfalardan farklı olduğunu ifade eder.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


Üstbilgi ve altbilginin belge ölçeklemesiyle ölçeklenip ölçeklenmediğini gösterir. Yalnızca Excel 2007 için geçerlidir.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


Bu özellik False ise, FitToPagesWide ve FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol eder.

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




### setAutoFirstPageNumber(boolean value) {#setAutoFirstPageNumber-boolean-}
```
public void setAutoFirstPageNumber(boolean value)
```


İlk sayfa numarasının otomatik olarak atanıp atanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


Belge öğelerinin siyah beyaz basılıp basılmayacağını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


Alt kenar boşluğunun boyutunu santimetre cinsinden temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


Alt kenar boşluğunun boyutunu inç cinsinden temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


Sayfanın yatay olarak ortalanıp ortalanmayacağını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


Sayfanın dikey olarak ortalanıp ortalanmayacağını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


Excel dosyasının çift sayfa altbilgisini biçimlendiren bir betik ayarlar. Yalnızca IsHFDiffOddEven true olduğunda Excel 2007'de etkilidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| footerScript | java.lang.String | Altbilgi biçim betiği. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


Excel dosyasının çift sayfa üstbilgisini biçimlendiren bir betik ayarlar. Yalnızca IsHFDiffOddEven true olduğunda Excel 2007'de etkilidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| headerScript | java.lang.String | Üstbilgi biçim betiği. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


Bir Excel dosyasının ilk sayfa alt bilgisini biçimlendiren bir betik ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| footerScript | java.lang.String | Altbilgi biçim betiği. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


Excel dosyasının ilk sayfa üstbilgisini biçimlendiren bir betik ayarlar. Yalnızca IsHFDiffFirst true olduğunda Excel 2007'de etkilidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| headerScript | java.lang.String | Üstbilgi biçim betiği. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


Bu sayfa yazdırıldığında kullanılacak birinci sayfa numarasını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


Çalışma sayfasının yazdırıldığında ölçekleneceği sayfa sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| geniş | int | Sayfa genişliği. |
| uzun | int | Sayfa yüksekliği. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


Çalışma sayfasının yazdırıldığında kaç sayfa yüksekliğine ölçekleneceğini temsil eder. Varsayılan değer 1'dir.

**Remarks**

Tüm satırları tek bir sayfaya sığdırmak istiyorsanız FitToPagesWide'ı sıfır olarak ayarlamanız gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


Çalışma sayfasının yazdırıldığında kaç sayfa genişliğine ölçekleneceğini temsil eder. Varsayılan değer 1'dir.

**Remarks**

Tüm sütunları tek bir sayfaya sığdırmak istiyorsanız FitToPagesTall'ı sıfır olarak ayarlamanız gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


Excel dosyasının altbilgisini biçimlendiren bir betik ayarlar.

**Remarks**

Betik komutları:

| Komut | Açıklama |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Geçerli sayfa numarası\u9286\u20ac |
| &N | Sayfa sayısı\u9286\u20ac |
| &D | Geçerli tarih\u9286\u20ac |
| &T | Geçerli zaman |
| &A | Sayfa adı |
| &F | Yol olmadan dosya adı |
| &\"<FontName>\" | Yazı tipi adı, örneğin: &\"Arial\" |
| &\"<FontName>, <FontStyle>\" | Yazı tipi adı ve yazı tipi stili, örneğin: &\"Arial,Bold\" |
| &<FontSize> | Yazı tipi boyutu. Bu komut, başlıkta yazdırılacak düz bir sayı ile takip edilirse, yazı tipi yüksekliğinden bir boşluk karakteri ile ayrılacaktır. |
| &K<RRGGBB> | Yazı tipi rengi, örneğin(KIRMIZI): &KFF0000 |
| &G | Görüntü betiği |

Örneğin: \"&Arial,Bold&8Footer Note\"

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| footerScript | java.lang.String | Altbilgi biçim betiği. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


Bir çalışma sayfasının altbilgisine bir resim ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| footerPicture | byte[] | Görüntü verisi. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


Üstbilgi ve altbilgi kenar boşluklarının sayfa kenar boşluklarıyla hizalanıp hizalanmadığını gösterir. Bu özellik true ise, sol üstbilgi ve altbilgi sol kenar boşluğuyla, sağ üstbilgi ve altbilgi sağ kenar boşluğuyla hizalanır. Bu seçenek varsayılan olarak etkindir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


Doğru, ilk sayfanın üst bilgi/alt bilgisinin diğer sayfalardan farklı olduğunu ifade eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


Doğru, tek sayfaların üst bilgi/alt bilgisinin diğer tek sayfalardan farklı olduğunu ifade eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


Üstbilgi ve altbilginin belge ölçeklemesiyle ölçeklenip ölçeklenmediğini gösterir. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


Excel dosyasının üstbilgisini biçimlendiren bir betik ayarlar.

**Remarks**

Betik komutları:

| Komut | Açıklama |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Geçerli sayfa numarası\u9286\u20ac |
| &N | Sayfa sayısı\u9286\u20ac |
| &D | Geçerli tarih\u9286\u20ac |
| &T | Geçerli zaman |
| &A | Sayfa adı |
| &F | Yol olmadan dosya adı |
| &\"<FontName>\" | Yazı tipi adı, örneğin: &\"Arial\" |
| &\"<FontName>, <FontStyle>\" | Yazı tipi adı ve yazı tipi stili, örneğin: &\"Arial,Bold\" |
| &<FontSize> | Yazı tipi boyutu. Bu komut, başlıkta yazdırılacak düz bir sayı ile takip edilirse, yazı tipi yüksekliğinden bir boşluk karakteri ile ayrılacaktır. |
| &K<RRGGBB> | Yazı tipi rengi, örneğin(KIRMIZI): &KFF0000 |
| &G | Görüntü betiği |

Örneğin: \"&Arial,Bold&8Header Note\"

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| headerScript | java.lang.String | Üstbilgi biçim betiği. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


Bir çalışma sayfasının üstbilgisine bir resim ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| headerPicture | byte[] | Görüntü verisi. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Sol kenar boşluğunun boyutunu santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


Sol kenar boşluğunun boyutunu inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Microsoft Excel'in büyük bir çalışma sayfasını yazdırırken sayfaları numaralandırmak için kullandığı sıralamayı temsil eder.

Bkz. [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Sayfa yazdırma yönünü temsil eder.

Bak [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Kağıdın boyutunu temsil eder.

Bakınız [PaperSizeType](../../com.aspose.cells/papersizetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


Bu özellik False ise, FitToPagesWide ve FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


Bir çalışma sayfasının üstbilgi/altbilgisine bir resim ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isFirst | boolean | İlk sayfa başlık/altbilgi resminin ayarlanıp ayarlanmadığını gösterir. |
| isEven | boolean | Çift sayfa başlık/altbilgi resminin ayarlanıp ayarlanmadığını gösterir. |
| isHeader | boolean | Başlık/altbilgi resminin ayarlanıp ayarlanmadığını gösterir. |
| section | int | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| imageData | byte[] | Görüntü verisi. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


Yazdırılacak aralığı temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


Yorumların sayfa ile birlikte nasıl yazdırıldığını temsil eder.

Bakınız [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


Yazdırılacak kopya sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


Sayfanın grafik olmadan yazdırılıp yazdırılmayacağını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


Görüntülenen yazdırma hatası türünü belirtir.

Bak [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


Hücre ızgara çizgilerinin sayfada yazdırılıp yazdırılmayacağını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


Satır ve sütun başlıklarının bu sayfada yazdırılıp yazdırılmayacağını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


Yazdırma kalitesini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


Her sayfanın sol tarafında tekrarlanacak hücreleri içeren sütunları temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


Her sayfanın üst kısmında tekrarlanacak hücreleri içeren satırları temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


Varsayılan yazıcının ayarlarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Sağ kenar boşluğunun boyutunu, santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


Sağ kenar boşluğunun boyutunu, inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


Üst kenar boşluğunun boyutunu, santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


Üst kenar boşluğunun boyutunu, inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Yüzde olarak ölçek faktörünü temsil eder. 10 ile 400 arasında olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

