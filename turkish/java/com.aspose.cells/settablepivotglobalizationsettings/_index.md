---
title: "SettablePivotGlobalizationSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcının önceden tanımlı metinleri ayarlamasına/değiştirmesine olanak tanıyan PivotGlobalizationSettings uygulaması."
type: docs
url: /tr/java/com.aspose.cells/settablepivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
```
public class SettablePivotGlobalizationSettings extends PivotGlobalizationSettings
```

Kullanıcının önceden tanımlı metinleri ayarlamasına/değiştirmesine olanak tanıyan PivotGlobalizationSettings uygulaması.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SettablePivotGlobalizationSettings()](#SettablePivotGlobalizationSettings--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | Pivot gün grubunun sayı biçimini alır. |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | Veri pivot alanının görüntüleme adını alır. |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | 12 ayın tüm kısa biçimlendirilmiş dizesini alır. |
| [getTextOf24Hours()](#getTextOf24Hours--) | 24 saatin tüm yerel biçimlendirilmiş dizesini alır. |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | 4 çeyreğin yerel metnini alır. |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | 4 çeyreğin yerel metnini alır. |
| [getTextOfAll()](#getTextOfAll--) | PivotTable'daki "(All)" etiketi metnini alır. |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | "All Periods" ifadesinin yerelleştirilmiş metnini alır. |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | PivotTable'daki "Column Labels" etiketi metnini alır. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | PivotTable'daki değer alanı alan başlığının metnini alır. |
| [getTextOfDays()](#getTextOfDays--) | "Days" öğesinin yerel metnini alır. |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | PivotTable'daki "(blank)" etiketinin metnini alır. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | PivotTable'daki "Grand Total" etiketinin metnini alır. |
| [getTextOfHours()](#getTextOfHours--) | "Hours" öğesinin yerel metnini alır. |
| [getTextOfMinutes()](#getTextOfMinutes--) | "Minutes" öğesinin yerel metnini alır. |
| [getTextOfMonths()](#getTextOfMonths--) | "Months" öğesinin yerel metnini alır. |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | PivotTable'daki "(Multiple Items)" etiketinin metnini alır. |
| [getTextOfOr()](#getTextOfOr--) | "or" ifadesinin tüm yerel biçimlendirilmiş dizesini alır. |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | Belirtilen korumalı ad için metni alır. |
| [getTextOfProtection()](#getTextOfProtection--) | PivotTable içindeki koruma adını alır. |
| [getTextOfQuarters()](#getTextOfQuarters--) | "Quarters" öğesinin yerel metnini al. |
| [getTextOfRange()](#getTextOfRange--) | "Range" öğesinin yerel metnini alır. |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | PivotTable'daki "Row Labels" etiketinin metnini alır. |
| [getTextOfSeconds()](#getTextOfSeconds--) | "Seconds" öğesinin yerel metnini alır. |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | PivotTable'daki [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) türünün metnini alır. |
| [getTextOfTotal()](#getTextOfTotal--) | PivotTable'daki "Total" etiketinin metnini alır. |
| [getTextOfYears()](#getTextOfYears--) | "Years" öğesinin yerel metnini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setTextOfAll(String text)](#setTextOfAll-java.lang.String-) | PivotTable'daki "(All)" etiketinin metnini ayarlar. |
| [setTextOfColumnLabels(String text)](#setTextOfColumnLabels-java.lang.String-) | PivotTable'daki "Column Labels" etiketi metnini alır. |
| [setTextOfDataFieldHeader(String text)](#setTextOfDataFieldHeader-java.lang.String-) | PivotTable'daki değer alanı başlığının metnini ayarlar. |
| [setTextOfEmptyData(String text)](#setTextOfEmptyData-java.lang.String-) | PivotTable'daki "(blank)" etiketinin metnini ayarlar. |
| [setTextOfGrandTotal(String text)](#setTextOfGrandTotal-java.lang.String-) | PivotTable'daki "Grand Total" etiketinin metnini ayarlar. |
| [setTextOfMultipleItems(String text)](#setTextOfMultipleItems-java.lang.String-) | PivotTable'daki "(Multiple Items)" etiketinin metnini ayarlar. |
| [setTextOfProtectedName(String protectedName, String text)](#setTextOfProtectedName-java.lang.String-java.lang.String-) | Belirli korumalı ad için metni ayarlar. |
| [setTextOfRowLabels(String text)](#setTextOfRowLabels-java.lang.String-) | PivotTable'daki "Row Labels" etiketinin metnini ayarlar. |
| [setTextOfSubTotal(int subTotalType, String text)](#setTextOfSubTotal-int-java.lang.String-) | PivotTable'daki [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) tipinin metnini ayarlar. |
| [setTextOfTotal(String text)](#setTextOfTotal-java.lang.String-) | PivotTable'daki "Total" etiketinin metnini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettablePivotGlobalizationSettings() {#SettablePivotGlobalizationSettings--}
```
public SettablePivotGlobalizationSettings()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatOfDayGroup() {#getFormatOfDayGroup--}
```
public String getFormatOfDayGroup()
```


Pivot gün grubunun sayı biçimini alır. Yalnızca pivot alanı günlere göre gruplanırken kullanılır. Varsayılan değer "d-MMM";

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


Veri pivot alanının görüntüleme adını alır. Varsayılan biçim "Sum Of Field".

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Fonksiyon, pivot alanının değerlerini özetlemek için kullanılır. |
| ad | java.lang.String | Pivot alanının orijinal adı. |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


12 ayın tüm kısa biçimlendirilmiş dizesini alır.

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


24 saatin tüm yerel biçimlendirilmiş dizesini alır. Varsayılan değer 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM.

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


4 çeyreğin yerel metnini alır.

**Remarks**

26.9'dan önce varsayılan olarak Quarter1, Quarter2, Quarter3, Quarter4 döndürür. 26.9'dan itibaren varsayılan olarak Qtr1, Qtr2, Qtr3, Qtr4 döndürür.

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


4 çeyreğin yerel metnini alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetTextOf4Quarters() yöntemini kullanın. Bu özellik Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


PivotTable'daki "(All)" etiketi metnini alır.

**Returns:**
java.lang.String - "(All)" etiketinin metni
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


"All Periods" ifadesinin yerelleştirilmiş metnini alır.

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


PivotTable'daki "Column Labels" etiketi metnini alır.

**Returns:**
java.lang.String - sütun etiketlerinin metni
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


PivotTable'daki değer alanı alan başlığının metnini alır.

**Returns:**
java.lang.String - veri alanı başlık adının metni
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


"Days" öğesinin yerel metnini alır.

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


PivotTable'daki "(blank)" etiketinin metnini alır.

**Returns:**
java.lang.String - boş veri metni
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


PivotTable'daki "Grand Total" etiketinin metnini alır.

**Returns:**
java.lang.String - "Grand Total" etiketinin metni
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


"Hours" öğesinin yerel metnini alır.

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


"Minutes" öğesinin yerel metnini alır.

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


"Months" öğesinin yerel metnini alır.

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


PivotTable'daki "(Multiple Items)" etiketinin metnini alır.

**Returns:**
java.lang.String - "(Multiple Items)" etiketinin metni
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


"or" ifadesinin tüm yerel biçimlendirilmiş dizesini alır.

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


Belirtilen korumalı ad için metni alır.

**Remarks**

Ms Excel'de, bazı adların PivotTable'daki PivotFields adı olarak kullanılması izin verilmez. Bunlar bölgeye göre farklılık gösterir, kullanıcı kullanılan bölgeye göre açıkça belirtebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| protectedName | java.lang.String | PivotTable'daki korumalı ad. |

**Returns:**
java.lang.String - PivotTable'ın yerel korunan adları
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


PivotTable içindeki koruma adını alır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotGlobalizationSettings.GetTextOfProtectedName(string) yöntemini kullanın. Bu özellik Mart 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String - PivotTable'ın koruma adı
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


"Quarters" öğesinin yerel metnini al.

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


"Range" öğesinin yerel metnini alır.

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


PivotTable'daki "Row Labels" etiketinin metnini alır.

**Returns:**
java.lang.String - satır etiketlerinin metni
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


"Seconds" öğesinin yerel metnini alır.

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


PivotTable'daki [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) türünün metnini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Bu [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - verilen tipin metni
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


PivotTable'daki "Total" etiketinin metnini alır. PivotTable veri alanında iki veya daha fazla PivotField içerdiğinde bu yöntemi geçersiz kılmanız gerekir.

**Returns:**
java.lang.String - "Total" etiketinin metni
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


"Years" öğesinin yerel metnini alır.

**Returns:**
java.lang.String -
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




### setTextOfAll(String text) {#setTextOfAll-java.lang.String-}
```
public void setTextOfAll(String text)
```


PivotTable'daki "(All)" etiketinin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | özel metin |

### setTextOfColumnLabels(String text) {#setTextOfColumnLabels-java.lang.String-}
```
public void setTextOfColumnLabels(String text)
```


PivotTable'daki "Column Labels" etiketi metnini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Sütun etiketlerinin metni |

### setTextOfDataFieldHeader(String text) {#setTextOfDataFieldHeader-java.lang.String-}
```
public void setTextOfDataFieldHeader(String text)
```


PivotTable'daki değer alanı başlığının metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Veri alanı başlık adının metni |

### setTextOfEmptyData(String text) {#setTextOfEmptyData-java.lang.String-}
```
public void setTextOfEmptyData(String text)
```


PivotTable'daki "(blank)" etiketinin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Boş veri metni |

### setTextOfGrandTotal(String text) {#setTextOfGrandTotal-java.lang.String-}
```
public void setTextOfGrandTotal(String text)
```


PivotTable'daki "Grand Total" etiketinin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | özel metin |

### setTextOfMultipleItems(String text) {#setTextOfMultipleItems-java.lang.String-}
```
public void setTextOfMultipleItems(String text)
```


PivotTable'daki "(Multiple Items)" etiketinin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | özel metin |

### setTextOfProtectedName(String protectedName, String text) {#setTextOfProtectedName-java.lang.String-java.lang.String-}
```
public void setTextOfProtectedName(String protectedName, String text)
```


Belirli korumalı ad için metni ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| protectedName | java.lang.String | PivotTable'daki korumalı ad. |
| metin | java.lang.String | PivotTable'ın yerel korumalı adları. |

### setTextOfRowLabels(String text) {#setTextOfRowLabels-java.lang.String-}
```
public void setTextOfRowLabels(String text)
```


PivotTable'daki "Row Labels" etiketinin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Satır etiketlerinin metni |

### setTextOfSubTotal(int subTotalType, String text) {#setTextOfSubTotal-int-java.lang.String-}
```
public void setTextOfSubTotal(int subTotalType, String text)
```


PivotTable'daki [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) tipinin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Bu [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| metin | java.lang.String | Verilen tipin metni |

### setTextOfTotal(String text) {#setTextOfTotal-java.lang.String-}
```
public void setTextOfTotal(String text)
```


PivotTable'daki "Total" etiketinin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | özel metin |

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

