---
title: "PivotFieldGroupOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pivot alanı gruplama ayarları için seçenekler."
type: docs
url: /tr/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

Pivot alanı gruplama ayarları için seçenekler.

**Example**

```
         // Load the sample workbook
         Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
         // Access the second worksheet and its pivot table
         PivotTable pt = wb.getWorksheets().get(1).getPivotTables().get(0);
         // Group the first row field (a date field) by months and quarters
         PivotFieldGroupOptions options = new PivotFieldGroupOptions();
         options.setStartDate(new DateTime(2008, 1, 1));
         options.setEndDate(new DateTime(2008, 9, 5));
         options.setGroupTypes(new /*PivotGroupByType*/int[] { PivotGroupByType.MONTHS, PivotGroupByType.QUARTERS });
         pt.getRowFields().get(0).group(options);
         // Calculate the pivot table data and save the output file
         pt.calculateData();
         wb.save("outputGroupPivotFieldsInPivotTable.xlsx");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | Ayrık grup öğelerini alır. |
| [getEndDate()](#getEndDate--) | Gruplama aralığının son değerini alır. |
| [getEndNumber()](#getEndNumber--) | Gruplama aralığının son değerini alır. |
| [getGroupType()](#getGroupType--) | Pivot alanı için grup türünü alır. |
| [getGroupTypes()](#getGroupTypes--) | Pivot alanı için grup türünü alır. |
| [getInterval()](#getInterval--) | Her grup için aralık boyutunu alır. |
| [getNewPivotField()](#getNewPivotField--) | Gruplamadan sonra yeni pivot alanlarının oluşturulup oluşturulmayacağını gösteren bir değeri alır. |
| [getStartDate()](#getStartDate--) | Gruplama aralığının başlangıç değerini alır. |
| [getStartNumber()](#getStartNumber--) | Gruplama aralığının başlangıç değerini alır. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | Son değerin otomatik olarak belirlenip belirlenmediğini gösteren bir değeri alır. |
| [isAutoStart()](#isAutoStart--) | Başlangıç değerinin otomatik olarak belirlenip belirlenmediğini gösteren bir değeri alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | Son değerin otomatik olarak belirlenip belirlenmeyeceğini gösteren bir değeri ayarlar. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | Başlangıç değerinin otomatik olarak belirlenip belirlenmeyeceğini gösteren bir değeri ayarlar. |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | Ayrık grup öğelerini ayarlar. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | Gruplama aralığının son değerini ayarlar. |
| [setEndNumber(double value)](#setEndNumber-double-) | Gruplama aralığının son değerini ayarlar. |
| [setGroupType(int value)](#setGroupType-int-) | Pivot alanı için grup türünü ayarlar. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | Pivot alanı için grup türünü ayarlar. |
| [setInterval(double value)](#setInterval-double-) | Her grup için aralık boyutunu ayarlar. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | Gruplamadan sonra yeni pivot alanlarının oluşturulup oluşturulmayacağını gösteren bir değeri ayarlar. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Gruplama aralığının başlangıç değerini ayarlar. |
| [setStartNumber(double value)](#setStartNumber-double-) | Gruplama aralığının başlangıç değerini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupOptions() {#PivotFieldGroupOptions--}
```
public PivotFieldGroupOptions()
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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


Ayrık grup öğelerini alır.

**Remarks**

Bu özellik ayarlanmışsa,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


Gruplama aralığının son değerini alır.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


Gruplama aralığının son değerini alır.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


Pivot alanı için gruplama türünü alır. Yalnızca tarih saat pivot alanı için gruplama.

Bak [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Example**

```
         //init
         PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
         // Group by year and month together
         /*PivotGroupByType*/int pivotGroupByType = pivotFieldGroupOptions.getGroupType();
         pivotGroupByType = PivotGroupByType.YEARS | PivotGroupByType.MONTHS;
         pivotFieldGroupOptions.setGroupType(pivotGroupByType);
```

**Returns:**
int
### getGroupTypes() {#getGroupTypes--}
```
public int[] getGroupTypes()
```


Pivot alanı için grup türünü alır.

Bak [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

Bu özellikteki sıralama yok sayılacaktır. Birden fazla grup türü belirtildiğinde, temel grup alanları artan sırada eklenir ve grup alanı satır/sütun bölgesine azalan sırada gösterilir (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


Her grup için aralık boyutunu alır.

**Remarks**

Yalnızca sayı ve gün grubu için.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


Gruplamadan sonra yeni pivot alanlarının oluşturulup oluşturulmayacağını gösteren bir değeri alır.

**Remarks**

Açıkça ayarlanmamışsa, varsayılan değer sayısal gruplama için false ve tarih-saat gruplama için true, ayrık grup için true'dur. Yalnızca temel alanın ilk yeni grup pivot alanı için çalışır.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Gruplama aralığının başlangıç değerini alır.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


Gruplama aralığının başlangıç değerini alır.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoEnd() {#isAutoEnd--}
```
public boolean isAutoEnd()
```


Son değerin otomatik olarak belirlenip belirlenmediğini gösteren bir değeri alır.

**Remarks**

Eğer [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) veya [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) ayarlanmışsa, bu özellik false olacaktır.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


Başlangıç değerinin otomatik olarak belirlenip belirlenmediğini gösteren bir değeri alır.

**Remarks**

Eğer [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) veya [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) ayarlanmışsa, bu özellik false olacaktır.

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




### setAutoEnd(boolean value) {#setAutoEnd-boolean-}
```
public void setAutoEnd(boolean value)
```


Son değerin otomatik olarak belirlenip belirlenmeyeceğini gösteren bir değeri ayarlar.

**Remarks**

Eğer [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) veya [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) ayarlanmışsa, bu özellik false olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


Başlangıç değerinin otomatik olarak belirlenip belirlenmeyeceğini gösteren bir değeri ayarlar.

**Remarks**

Eğer [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) veya [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) ayarlanmışsa, bu özellik false olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


Ayrık grup öğelerini ayarlar.

**Remarks**

Bu özellik ayarlanmışsa,[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


Gruplama aralığının son değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


Gruplama aralığının son değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


Pivot alanı için gruplama türünü ayarlar. Yalnızca tarih saat pivot alanı için gruplama.

Bak [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


Pivot alanı için grup türünü ayarlar.

Bak [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

Bu özellikteki sıralama yok sayılacaktır. Birden fazla grup türü belirtildiğinde, temel grup alanları artan sırada eklenir ve grup alanı satır/sütun bölgesine azalan sırada gösterilir (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


Her grup için aralık boyutunu ayarlar.

**Remarks**

Yalnızca sayı ve gün grubu için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


Gruplamadan sonra yeni pivot alanlarının oluşturulup oluşturulmayacağını gösteren bir değeri ayarlar.

**Remarks**

Açıkça ayarlanmamışsa, varsayılan değer sayısal gruplama için false ve tarih-saat gruplama için true, ayrık grup için true'dur. Yalnızca temel alanın ilk yeni grup pivot alanı için çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Gruplama aralığının başlangıç değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


Gruplama aralığının başlangıç değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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

