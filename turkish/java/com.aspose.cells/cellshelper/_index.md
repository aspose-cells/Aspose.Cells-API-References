---
title: "CellsHelper"
second_title: "Aspose.Cells for Java API Referansı"
description: "Yardımcı işlevler sağlar."
type: docs
url: /tr/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

Yardımcı işlevler sağlar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | Eklenti işlevi ekle. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Hücrenin adını satır ve sütun indekslerine göre alır. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | Hücrenin satır ve sütun indekslerini adına göre alır. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Sütun indeksine göre sütun adını alır. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Sütun adına göre sütun indeksini alır. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | Hücrenin A1 formülünü r1c1 formülüne dönüştürür. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | Hücrenin r1c1 formülünü A1 formülüne dönüştürür. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | Bazı dış formül referansları tarafından kullanılan alternatif başlangıç yolunu alır. |
| [getCacheFolder()](#getCacheFolder--) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü alır. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | Özel uygulama ile örnekler oluşturmak için fabrikayı alır. |
| [getDPI()](#getDPI--) | Makinenin DPI değerini alır. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | Double değerini tarih saat değerine dönüştürür. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | Tarih saat değerini double değerine dönüştürür. |
| [getLibraryPath()](#getLibraryPath--) | Bazı dış formül referansları tarafından kullanılan kütüphane yolunu alır. |
| [getSignificantDigits()](#getSignificantDigits--) | Önemli basamak sayısını alır. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Sayısal değerleri çıktıya verirken kullanılan varsayılan önemli basamak tipini alır. |
| [getStartupPath()](#getStartupPath--) | Bazı dış formül referansları tarafından kullanılan başlangıç yolunu alır. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | Metnin genişliğini nokta biriminde al. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | Çalışma kitabında kullanılan tüm renkleri alır. |
| [getVersion()](#getVersion--) | Sürüm numarasını al. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | Bu özelliği, Azure, AWSLambda vb. gibi bir bulut platformunda çalıştırırken True olarak ayarlayın, |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | Bazı büyük xls dosyalarını tek bir xls dosyasına birleştirir. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | Sayfa adının tek tırnak içinde olup olmayacağını belirtir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | Satır indeksine göre satır adını alır. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | Satır adına göre satır indeksini alır. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | Bazı dış formül referansları tarafından kullanılan alternatif başlangıç yolunu ayarlar. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü ayarlar. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | Bu özelliği, Azure, AWSLambda vb. gibi bir bulut platformunda çalıştırırken True olarak ayarlayın, |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | Özel uygulama ile örnekler oluşturmak için fabrikayı ayarlar. |
| [setDPI(double value)](#setDPI-double-) | Makinenin DPI değerini alır. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | Bazı dış formül referansları tarafından başvurulan kütüphane yolunu ayarlar. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Önemli basamak sayısını ayarlar. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Sayısal değerlerin çıktısı için varsayılan önemli basamak türünü ayarlar. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | Bazı dış formül referansları tarafından başvurulan başlangıç yolunu ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


Eklenti işlevi ekle.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen WorksheetCollection.RegisterAddInFunction() yöntemlerini kullanın. Bu yöntem, Ocak 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fonksiyon | java.lang.String | Fonksiyon adı. |
| minCountOfParameters | int | Bu fonksiyonun gerektirdiği minimum parametre sayısı |
| maxCountOfParameters | int | Bu fonksiyonun izin verdiği maksimum parametre sayısı. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). Fonksiyonun beklenen parametre türü |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). Fonksiyon değer türü. |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Hücrenin adını satır ve sütun indekslerine göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Hücre adı.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


Hücrenin satır ve sütun indekslerini adına göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı |

**Returns:**
int[] - [0] satır indeksi ve [1] sütun indeksidir.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Sütun indeksine göre sütun adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi. |

**Returns:**
java.lang.String - Sütun adı.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Sütun adına göre sütun indeksini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnName | java.lang.String | Sütun adı. |

**Returns:**
int - Sütun indeksi.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


Hücrenin A1 formülünü r1c1 formülüne dönüştürür.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Worksheet.ConvertFormulaReferenceStyle() yöntemini kullanın. Bu özellik, Ağustos 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | A1 formülü. |
| satır | int | Hücrenin satır indeksi. |
| sütun | int | Hücrenin sütun indeksi. |

**Returns:**
java.lang.String - R1C1 formülü.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


Hücrenin r1c1 formülünü A1 formülüne dönüştürür.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Worksheet.ConvertFormulaReferenceStyle() yöntemini kullanın. Bu özellik, Ağustos 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| r1c1Formula | java.lang.String | r1c1 formülü. |
| satır | int | Hücrenin satır indeksi. |
| sütun | int | Hücrenin sütun indeksi. |

**Returns:**
java.lang.String - A1 formülü.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa, onu döndürür. Aksi takdirde, uzunluk sınırı aşılırsa dize kesilir ve geçersiz karakterler ' ' ile değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| nameProposal | java.lang.String | kullanılacak sayfa adı |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa, onu döndürür. Aksi takdirde, uzunluk sınırı aşılırsa dize kesilir ve geçersiz karakterler verilen karakterle değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| nameProposal | java.lang.String | kullanılacak sayfa adı |
| replaceChar | char | verilen sayfa adındaki geçersiz karakterleri değiştirmek için kullanılacak karakter |

**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


Bazı dış formül referansları tarafından kullanılan alternatif başlangıç yolunu alır.

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü alır.

**Remarks**

Önbellek dosyaları genellikle bellek performansı düşünülerek bazı özellikler için kullanılır; örneğin büyük veri setini xls dosyasına kaydetmek veya hücre modeli için dosya önbelleğiyle bellek modunu kullanmak gibi.

**Returns:**
java.lang.String - Belirtilen önbellek dosyaları klasörü. Belirtilmemişse, null döndürülür ve gerektiğinde sistemin geçici yolu kullanılır.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


Özel uygulama ile örnekler oluşturmak için fabrikayı alır.

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Makinenin DPI değerini alır.

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


Double değerini tarih saat değerine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| doubleValue | double | Double değeri. |
| date1904 | boolean | 1904 tarih sistemi. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


Tarih saat değerini double değerine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Tarih ve saat. |
| date1904 | boolean | 1904 tarih sistemi. |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


Bazı dış formül referansları tarafından kullanılan kütüphane yolunu alır.

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


Önemli basamak sayısını alır. Varsayılan değer 17'dir.

**Remarks**

Şu anda yalnızca 15 veya 17 olabilir. NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--) adresini kullanın. Bu özellik, Haziran 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


Sayısal değerleri çıkartırken kullanılan varsayılan önemli basamak tipini alır. Varsayılan değer [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Bakınız [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


Bazı dış formül referansları tarafından kullanılan başlangıç yolunu alır.

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


Metnin genişliğini nokta biriminde al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Metin. |
| font | [Font](../../com.aspose.cells/font) | Metnin yazı tipi. |
| ölçekleme | double | Metnin ölçeklendirilmesi. |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


Çalışma kitabında kullanılan tüm renkleri alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Çalışma kitabı nesnesi. |

**Returns:**
com.aspose.cells.Color[] - Kullanılan renkler.
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Sürüm numarasını al.

**Returns:**
java.lang.String - Yayın sürümü.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


Bu özelliği, Azure, AWSLambda vb. gibi bir bulut platformunda çalıştırırken True olarak ayarlayın,

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


Bazı büyük xls dosyalarını tek bir xls dosyasına birleştirir.

**Remarks**

Bu yöntem yalnızca veri, stil ve formüllerin yeni dosyaya birleştirilmesini destekler. Önbellek dosyası bazı geçici verileri depolamak için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyalar | java.lang.String[] | Dosyalar. |
| cachedFile | java.lang.String | Önbellek dosyası. |
| destFile | java.lang.String | Hedef dosya. |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


Sayfa adının tek tırnak içinde olup olmayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Sayfanın adı |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


Satır indeksine göre satır adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |

**Returns:**
java.lang.String - Satır adı.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


Satır adına göre satır indeksini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowName | java.lang.String | Satır adı. |

**Returns:**
int - Satır indeksi.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


Bazı dış formül referansları tarafından kullanılan alternatif başlangıç yolunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü ayarlar.

**Remarks**

Önbellek dosyaları genellikle bellek performansı düşünülerek bazı özellikler için kullanılır; örneğin büyük veri setini xls dosyasına kaydetmek veya hücre modeli için dosya önbelleğiyle bellek modunu kullanmak gibi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| önbellek | java.lang.String | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasör. |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


Bu özelliği, Azure, AWSLambda vb. gibi bir bulut platformunda çalıştırırken True olarak ayarlayın,

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


Özel uygulama ile örnekler oluşturmak için fabrikayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Makinenin DPI değerini alır.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


Bazı dış formül referansları tarafından başvurulan kütüphane yolunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


Önemli basamak sayısını ayarlar. Varsayılan değer 17'dir.

**Remarks**

Şu anda yalnızca 15 veya 17 olabilir. NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--) adresini kullanın. Bu özellik, Haziran 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


Sayısal değerlerin çıktısı için varsayılan önemli basamak tipini ayarlar. Varsayılan değer [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17) dir.

Bakınız [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


Bazı dış formül referansları tarafından başvurulan başlangıç yolunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

