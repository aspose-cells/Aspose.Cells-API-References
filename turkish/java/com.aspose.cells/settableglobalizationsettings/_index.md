---
title: "SettableGlobalizationSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcının önceden tanımlı metinleri ayarlamasına/değiştirmesine olanak tanıyan GlobalizationSettings uygulaması."
type: docs
url: /tr/java/com.aspose.cells/settableglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
```
public class SettableGlobalizationSettings extends GlobalizationSettings
```

Kullanıcının önceden tanımlı metinleri ayarlamasına/değiştirmesine olanak tanıyan GlobalizationSettings uygulaması.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SettableGlobalizationSettings()](#SettableGlobalizationSettings--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Belirli sıralama kurallarına göre iki dize değerini karşılaştırır. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | PivotTable'daki "(All)" etiketinin adını alır. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Hücrenin boolean değerinin görüntüleme dizesi değerini alır. |
| [getChartSettings()](#getChartSettings--) | Grafik için küreselleştirme ayarlarını alır. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Belirli sıralama kurallarına göre dizeyi karşılaştırılabilir bir nesneye dönüştürür. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | PivotTable'daki "Column Labels" etiketinin adını alır. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Formülde dizinin satır verisindeki öğeler için ayırıcıyı alır. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Yorum başlığı tipine göre yerel ayara bağlı yorum başlığı adını alır. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | PivotTable'daki değer alanı başlığının adını alır. |
| [getDefaultSheetName()](#getDefaultSheetName--) | Çalışma sayfasını otomatik eklemek için varsayılan sayfa adını alır. |
| [getEmptyDataName()](#getEmptyDataName--) | PivotTable içindeki "(blank)" etiketinin adını alır. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Hücrenin hata değerinin görüntüleme dizesi değerini alır. |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Fonksiyonun genel toplam adını alır. |
| [getListSeparator()](#getListSeparator--) | Liste, fonksiyon parametreleri, ... vb. için ayırıcıyı alır. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Verilen standart metne göre yerel ayara bağlı olarak yerleşik Ad için metni alır. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını alır. |
| [getMultipleItemsName()](#getMultipleItemsName--) | PivotTable içindeki "(Multiple Items)" etiketinin adını alır. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | PivotTable içindeki "Grand Total" etiketinin adını alır. |
| [getPivotSettings()](#getPivotSettings--) | Pivot tablo için küreselleştirme ayarlarını alır. |
| [getPivotTotalName()](#getPivotTotalName--) | PivotTable içindeki "Total" etiketinin adını alır. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | PivotTable içindeki koruma adını alır. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | PivotTable içindeki "Row Labels" etiketinin adını alır. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | Formüldeki dizi verisindeki satırlar için ayırıcıyı alır. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | Verilen yerel ayara bağlı metne göre yerleşik Adın standart metnini alır. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | Verilen yerel yazı tipi stiline göre Başlık/Altbilgi için standart İngilizce yazı tipi stili adını (Regular, Bold, Italic) alır. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | PivotTable içindeki [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) tipinin adını alır. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | Referans verilen tablodaki tüm satırları içeren tablo satırlarının tip adını alır. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | Referans verilen tablodaki mevcut satırı içeren tablo satırlarının tip adını alır. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | Referans verilen tablonun veri bölgesini içeren tablo satırlarının tip adını alır. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | Tablo başlığını içeren tablo satırlarının tip adını alır. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | Referans verilen tablonun toplam satırını içeren tablo satırlarının tip adını alır. |
| [getTotalName(int functionType)](#getTotalName-int-) | Belirli fonksiyonun toplam adını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBooleanValueString(boolean bv, String name)](#setBooleanValueString-boolean-java.lang.String-) | Hücrenin boolean değerinin görüntüleme dizesi değerini ayarlar. |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Chart için küreselleştirme ayarlarını ayarlar. |
| [setColumnSeparatorOfFormulaArray(char c)](#setColumnSeparatorOfFormulaArray-char-) | Formülde dizi satır verilerindeki öğeler için ayırıcıyı ayarlar. |
| [setCommentTitleName(int type, String name)](#setCommentTitleName-int-java.lang.String-) | Yorum başlığı tipine göre yerel ayara bağlı yorum başlığı adını alır. |
| [setGrandTotalName(int functionType, String name)](#setGrandTotalName-int-java.lang.String-) | Belirli işlevin toplam adını ayarlar. |
| [setListSeparator(char c)](#setListSeparator-char-) | Liste, işlev parametreleri vb. için ayırıcıyı ayarlar. |
| [setLocalBuiltInName(String standardName, String localName, boolean bidirectional)](#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-) | Verilen standart ad metniyle yerleşik ad için yerel ayara bağlı metni ayarlar. |
| [setLocalFunctionName(String standardName, String localName, boolean bidirectional)](#setLocalFunctionName-java.lang.String-java.lang.String-boolean-) | Verilen standart işlev adına karşılık gelen yerel ayara bağlı işlev adını ayarlar. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Özet tablo için küreselleştirme ayarlarını ayarlar. |
| [setRowSeparatorOfFormulaArray(char c)](#setRowSeparatorOfFormulaArray-char-) | Formülde dizi verilerindeki satırlar için ayırıcıyı ayarlar. |
| [setStandardBuiltInName(String localName, String standardName, boolean bidirectional)](#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-) | Verilen standart işlev adına göre yerel ayara bağlı işlev adını ayarlar. |
| [setStandardFunctionName(String localName, String standardName, boolean bidirectional)](#setStandardFunctionName-java.lang.String-java.lang.String-boolean-) | Verilen standart işlev adına göre yerel ayara bağlı işlev adını ayarlar. |
| [setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)](#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-) | Verilen standart işlev adına göre yerel ayara bağlı işlev adını ayarlar. |
| [setTableRowTypeOfAll(String name)](#setTableRowTypeOfAll-java.lang.String-) | Referans alınan tablodaki tüm satırları içeren tablo satırlarının tip adını ayarlar. |
| [setTableRowTypeOfCurrent(String name)](#setTableRowTypeOfCurrent-java.lang.String-) | Referans alınan tablodaki mevcut satırı içeren tablo satırlarının tip adını ayarlar. |
| [setTableRowTypeOfData(String name)](#setTableRowTypeOfData-java.lang.String-) | Referans alınan tablonun veri bölgesini içeren tablo satırlarının tip adını ayarlar. |
| [setTableRowTypeOfHeaders(String name)](#setTableRowTypeOfHeaders-java.lang.String-) | Tablo başlığını içeren tablo satırlarının tip adını ayarlar. |
| [setTableRowTypeOfTotals(String name)](#setTableRowTypeOfTotals-java.lang.String-) | Referans alınan tablonun toplam satırını içeren tablo satırlarının tip adını ayarlar. |
| [setTotalName(int functionType, String name)](#setTotalName-int-java.lang.String-) | Belirli işlevin toplam adını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettableGlobalizationSettings() {#SettableGlobalizationSettings--}
```
public SettableGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Belirli sıralama kurallarına göre iki dize değerini karşılaştırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| v1 | java.lang.String | ilk dize |
| v2 | java.lang.String | ikinci dize |
| ignoreCase | boolean | değerleri karşılaştırırken büyük/küçük harfe duyarlı olup olmadığı |

**Returns:**
int - İki karşılaştırılan öğe arasındaki sözcüksel ilişkiyi gösteren tamsayı
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


PivotTable'daki "(All)" etiketinin adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen GlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik Aralık 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - "(All)" etiketinin adı
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


Hücrenin boolean değerinin görüntüleme dizesi değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bv | boolean | boolean değer |

**Returns:**
java.lang.String - Varsayılan olarak "TRUE" doğru değer ve "FALSE" yanlış değer döndürür.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


Grafik için küreselleştirme ayarlarını alır.

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Belirli sıralama kurallarına göre dizeyi karşılaştırılabilir bir nesneye dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| v | java.lang.String | String değeri diğerleriyle karşılaştırılmalıdır. |
| ignoreCase | boolean | değerleri karşılaştırırken büyük/küçük harfe duyarlı olup olmadığı |

**Returns:**
java.lang.Comparable - Nesne, string değerlerini karşılaştırmak veya sıralamak için kullanılabilir.
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


PivotTable'daki "Column Labels" etiketinin adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - Sütun etiketlerinin adı
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


Formülde dizinin satır verisindeki öğeler için ayırıcıyı alır.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


Yorum başlığı tipine göre yerel ayara bağlı yorum başlığı adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). yorum başlığının türü |

**Returns:**
java.lang.String - yerel ayara bağlı yorum başlığı adı
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


PivotTable'daki değer alanı başlığının adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - Veri alanı başlık adının adı
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


Varsayılan sayfa adını otomatik olarak alır. Varsayılan "Sheet".

**Remarks**

Otomatik olarak eklenen (örneğin [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\#add--)) sayfanın adı, belirtilen adın artı sıra numarası olacaktır. Örneğin, Almanya kullanıcısı sayfa adının "Sheet2" yerine "Tabellenblatt2" olmasını isteyebilir. Bu durumda kullanıcı bu yöntemi "Tabellenblatt" döndürecek şekilde uygulayabilir.

**Returns:**
java.lang.String - otomatik olarak çalışma sayfası eklemek için varsayılan sayfa adı
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


PivotTable içindeki "(blank)" etiketinin adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - Boş veri adı
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


Hücrenin hata değerinin görüntüleme dizesi değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| err | java.lang.String | hata değerleri örneğin \#VALUE!,\#NAME? |

**Returns:**
java.lang.String - Varsayılan olarak hata değerini kendisini döndürür.
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Fonksiyonun genel toplam adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Fonksiyon türü. |

**Returns:**
java.lang.String - Fonksiyonun genel toplam adı.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


Liste, fonksiyon parametreleri, ... vb. için ayırıcıyı alır.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


Verilen standart metne göre yerel ayara bağlı olarak yerleşik Ad için metni alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) yerleşik Name'in metni. |

**Returns:**
java.lang.String - Yerel ayara bağlı metin. Yerel ayar, bu ayarların kullanıldığı Workbook tarafından belirtilmiştir.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) fonksiyon adı. |

**Returns:**
java.lang.String - Yerel ayara bağlı fonksiyon adı. Yerel ayar, bu ayarların kullanıldığı Workbook tarafından belirtilmiştir.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


PivotTable içindeki "(Multiple Items)" etiketinin adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - "(Multiple Items)" etiketinin adı
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


PivotTable içindeki "Grand Total" etiketinin adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - "Grand Total" etiketinin adı
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


Pivot tablo için küreselleştirme ayarlarını alır.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


PivotTable içinde "Total" etiketinin adını alır. PivotTable veri alanında iki veya daha fazla PivotField içerdiğinde bu yöntemi geçersiz kılmanız gerekir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - "Total" etiketinin adı
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


PivotTable içindeki koruma adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetTextOfProtectedName(string) yöntemini kullanın. Bu özellik Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - PivotTable'ın koruma adı
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


PivotTable içindeki "Row Labels" etiketinin adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - Satır etiketlerinin adı
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


Formüldeki dizi verisindeki satırlar için ayırıcıyı alır.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


Verilen yerel ayara bağlı metne göre yerleşik Adın standart metnini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localName | java.lang.String | Yerel ayara bağlı yerleşik Adın metni. Yerel ayar, bu ayarların kullanıldığı Çalışma Kitabı tarafından belirtilmiştir. |

**Returns:**
java.lang.String - Standart (en-US yerel ayarı) metin.
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localName | java.lang.String | Yerel ayara bağlı fonksiyon adı. Yerel ayar, bu ayarların kullanıldığı Çalışma Kitabı tarafından belirtilmiştir. |

**Returns:**
java.lang.String - Standart (en-US yerel ayarı) fonksiyon adı.
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


Verilen yerel yazı tipi stiline göre Başlık/Altbilgi için standart İngilizce yazı tipi stili adını (Regular, Bold, Italic) alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Üst Bilgi/Alt Bilgi için yerel ayara bağlı yazı tipi stili adı. |

**Returns:**
java.lang.String - Standart İngilizce yazı tipi stili adı (Normal, Kalın, İtalik)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


PivotTable içindeki [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) tipinin adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) türü |

**Returns:**
java.lang.String - [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) türünün adı
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Referans verilen tablodaki tüm satırları içeren tablo satırlarının tip adını alır.

**Returns:**
java.lang.String - tablo satırlarının tür adı
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Referans verilen tablodaki mevcut satırı içeren tablo satırlarının tip adını alır.

**Returns:**
java.lang.String - tablo satırlarının tür adı
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


Referans alınan tablonun veri bölgesinden oluşan tablo satırlarının tür adını alır. Varsayılan \"Data\" dır, bu yüzden formülde \"\\#Data\" tablonun veri bölgesini temsil eder.

**Returns:**
java.lang.String - tablo satırlarının tür adı
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


Tablo başlığından oluşan tablo satırlarının tür adını alır. Varsayılan \"Headers\" dır, bu yüzden formülde \"\\#Headers\" tablo başlığını temsil eder.

**Returns:**
java.lang.String - tablo satırlarının tür adı
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


Referans verilen tablonun toplam satırını içeren tablo satırlarının tip adını alır.

**Returns:**
java.lang.String - tablo satırlarının tür adı
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Belirli fonksiyonun toplam adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Fonksiyon türü. |

**Returns:**
java.lang.String - Fonksiyonun toplam adı
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBooleanValueString(boolean bv, String name) {#setBooleanValueString-boolean-java.lang.String-}
```
public void setBooleanValueString(boolean bv, String name)
```


Hücrenin boolean değerinin görüntüleme dizesi değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bv | boolean | boolean değer |
| ad | java.lang.String | boolean değerinin string değeri |

### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Chart için küreselleştirme ayarlarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setColumnSeparatorOfFormulaArray(char c) {#setColumnSeparatorOfFormulaArray-char-}
```
public void setColumnSeparatorOfFormulaArray(char c)
```


Formülde dizi satır verilerindeki öğeler için ayırıcıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | char | belirtilen ayırıcı |

### setCommentTitleName(int type, String name) {#setCommentTitleName-int-java.lang.String-}
```
public void setCommentTitleName(int type, String name)
```


Yorum başlığı tipine göre yerel ayara bağlı yorum başlığı adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). yorum başlığının türü |
| ad | java.lang.String | yerel ayara bağlı yorum başlığı adı |

### setGrandTotalName(int functionType, String name) {#setGrandTotalName-int-java.lang.String-}
```
public void setGrandTotalName(int functionType, String name)
```


Belirli işlevin toplam adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Fonksiyon türü. |
| ad | java.lang.String | Fonksiyonun genel toplam adı. |

### setListSeparator(char c) {#setListSeparator-char-}
```
public void setListSeparator(char c)
```


Liste, işlev parametreleri vb. için ayırıcıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | char | belirtilen ayırıcı |

### setLocalBuiltInName(String standardName, String localName, boolean bidirectional) {#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalBuiltInName(String standardName, String localName, boolean bidirectional)
```


Verilen standart ad metniyle yerleşik ad için yerel ayara bağlı metni ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | java.lang.String | Yerleşik adın standart (en-US yereli) ad metni. |
| localName | java.lang.String | Yerel bağımlı ad metni |
| bidirectional | boolean | Yerel ad metninin standart ad metnine otomatik olarak eşlenip eşlenmeyeceği. Doğru ise, yerel ad metni otomatik olarak standart ad metnine eşlenecek, böylece kullanıcı aynı standart ve yerel ad çifti için tekrar [setStandardBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardBuiltInName-String-String-boolean-) çağırmak zorunda kalmayacaktır. |

### setLocalFunctionName(String standardName, String localName, boolean bidirectional) {#setLocalFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalFunctionName(String standardName, String localName, boolean bidirectional)
```


Verilen standart işlev adına karşılık gelen yerel ayara bağlı işlev adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) fonksiyon adı. |
| localName | java.lang.String | Yerel bağımlı işlev adı |
| bidirectional | boolean | Yerel işlev adının standart işlev adına otomatik olarak eşlenip eşlenmeyeceği. Doğru ise, yerel ad otomatik olarak standart ada eşlenecek, böylece kullanıcı aynı standart ve yerel ad çifti için tekrar [setStandardFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardFunctionName-String-String-boolean-) çağırmak zorunda kalmayacaktır. |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Özet tablo için küreselleştirme ayarlarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

### setRowSeparatorOfFormulaArray(char c) {#setRowSeparatorOfFormulaArray-char-}
```
public void setRowSeparatorOfFormulaArray(char c)
```


Formülde dizi verilerindeki satırlar için ayırıcıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | char | belirtilen ayırıcı |

### setStandardBuiltInName(String localName, String standardName, boolean bidirectional) {#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardBuiltInName(String localName, String standardName, boolean bidirectional)
```


Verilen standart işlev adına göre yerel ayara bağlı işlev adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localName | java.lang.String | Yerel bağımlı işlev adı |
| standardName | java.lang.String | Standard(en-US locale) fonksiyon adı. |
| bidirectional | boolean | Standart ad metninin yerel ad metnine otomatik olarak eşlenip eşlenmeyeceği. Doğru ise, standart ad metni otomatik olarak yerel ad metnine eşlenecek, böylece kullanıcı aynı standart ve yerel ad çifti için tekrar [setLocalBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalBuiltInName-String-String-boolean-) çağırmak zorunda kalmayacaktır. |

### setStandardFunctionName(String localName, String standardName, boolean bidirectional) {#setStandardFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardFunctionName(String localName, String standardName, boolean bidirectional)
```


Verilen standart işlev adına göre yerel ayara bağlı işlev adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localName | java.lang.String | Yerel bağımlı işlev adı |
| standardName | java.lang.String | Standard(en-US locale) fonksiyon adı. |
| bidirectional | boolean | Standart işlev adının yerel işlev adına otomatik olarak eşlenip eşlenmeyeceği. Doğru ise, standart ad otomatik olarak yerel ada eşlenecek, böylece kullanıcı aynı standart ve yerel ad çifti için tekrar [setLocalFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalFunctionName-String-String-boolean-) çağırmak zorunda kalmayacaktır. |

### setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName) {#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-}
```
public void setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)
```


Verilen standart işlev adına göre yerel ayara bağlı işlev adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Üst Bilgi/Alt Bilgi için yerel ayara bağlı yazı tipi stili adı. |
| standardName | java.lang.String | Standard(en-US locale) fonksiyon adı. |

### setTableRowTypeOfAll(String name) {#setTableRowTypeOfAll-java.lang.String-}
```
public void setTableRowTypeOfAll(String name)
```


Referans alınan tablodaki tüm satırları içeren tablo satırlarının tip adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | tablo satırlarının tür adı |

### setTableRowTypeOfCurrent(String name) {#setTableRowTypeOfCurrent-java.lang.String-}
```
public void setTableRowTypeOfCurrent(String name)
```


Referans alınan tablodaki mevcut satırı içeren tablo satırlarının tip adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | tablo satırlarının tür adı |

### setTableRowTypeOfData(String name) {#setTableRowTypeOfData-java.lang.String-}
```
public void setTableRowTypeOfData(String name)
```


Referans alınan tablonun veri bölgesini içeren tablo satırlarının tip adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | tablo satırlarının tür adı |

### setTableRowTypeOfHeaders(String name) {#setTableRowTypeOfHeaders-java.lang.String-}
```
public void setTableRowTypeOfHeaders(String name)
```


Tablo başlığını içeren tablo satırlarının tip adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | tablo satırlarının tür adı |

### setTableRowTypeOfTotals(String name) {#setTableRowTypeOfTotals-java.lang.String-}
```
public void setTableRowTypeOfTotals(String name)
```


Referans alınan tablonun toplam satırını içeren tablo satırlarının tip adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | tablo satırlarının tür adı |

### setTotalName(int functionType, String name) {#setTotalName-int-java.lang.String-}
```
public void setTotalName(int functionType, String name)
```


Belirli işlevin toplam adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Fonksiyon türü. |
| ad | java.lang.String | Fonksiyonun toplam adı. |

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

