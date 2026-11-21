---
title: "PivotGlobalizationSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pivot tablolar için küreselleştirme ayarlarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotGlobalizationSettings
```

Pivot tablolar için küreselleştirme ayarlarını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PivotGlobalizationSettings()](#PivotGlobalizationSettings--) |  |
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
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotGlobalizationSettings() {#PivotGlobalizationSettings--}
```
public PivotGlobalizationSettings()
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

