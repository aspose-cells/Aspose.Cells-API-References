---
title: "PivotFieldSortSetting"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pivot alanlarını sıralama ayarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

Pivot alanlarını sıralama ayarını temsil eder.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Sort by the first data field ascending.
         rowField.sortBy(SortOrder.ASCENDING, 0, null);
 
         //Gets sort settings of the pivot field.
         PivotFieldSortSetting sortSetting = rowField.getSortSetting();
         System.out.println(sortSetting.getSortType());
         //do your business
 
         pivot.calculateData();
         book.save("out.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Satır veya sütunda bulunan değerlere göre sıralar. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Sıralanan alanın dizinini temsil eder |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | Sıralanan pivot satır türü. |
| [getSortBy()](#getSortBy--) | Sıralanan alanın dizinini temsil eder. |
| [getSortType()](#getSortType--) | [SortOrder](../../com.aspose.cells/sortorder) öğesini temsil eder. |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | Basit bir veri sıralama işleminin uygulanıp uygulanmayacağını gösterir. |
| [isSortByLabels()](#isSortByLabels--) | Alanı kendi başına mı yoksa veri alanına göre mi sıralayacağını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Sıralanan alanın dizinini temsil eder |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | Basit bir veri sıralama işleminin uygulanıp uygulanmayacağını gösterir. |
| [setSortBy(int value)](#setSortBy-int-) | Sıralanan alanın dizinini temsil eder. |
| [setSortType(int value)](#setSortType-int-) | [SortOrder](../../com.aspose.cells/sortorder) öğesini temsil eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCell() {#getCell--}
```
public String getCell()
```


Satır veya sütunda bulunan değerlere göre sıralar.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Sıralanan alanın dizinini temsil eder. -1, PivotField'in etiketlere göre sıralandığını, diğer değerler ise veri alanına göre sıralandığını gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotFieldSortSetting.SortBy özelliğini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


Sıralanan pivot satır türü.

[PivotLineType](../../com.aspose.cells/pivotlinetype) öğesine bakın.

**Remarks**

Bu alan etiketlere göre sıralanmadığında yalnızca çalışır.

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


Sıralanan alanın dizinini temsil eder. -1 değeri, pivot öğesinin kendi değerlerine göre sıralandığını gösterir. Sıfır veya daha büyük olduğunda, veri bölgesindeki veri alanının dizinini temsil eder.

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


[SortOrder](../../com.aspose.cells/sortorder) öğesini temsil eder.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSimpleSort() {#isSimpleSort--}
```
public boolean isSimpleSort()
```


Basit bir veri sıralama işleminin uygulanıp uygulanmayacağını gösterir.

**Remarks**

Varsayılan değer true'tır.

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


Alanı kendi başına mı yoksa veri alanına göre mi sıralayacağını gösterir.

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




### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Sıralanan alanın dizinini temsil eder. -1, PivotField'in etiketlere göre sıralandığını, diğer değerler ise veri alanına göre sıralandığını gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotFieldSortSetting.SortBy özelliğini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


Basit bir veri sıralama işleminin uygulanıp uygulanmayacağını gösterir.

**Remarks**

Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


Sıralanan alanın dizinini temsil eder. -1 değeri, pivot öğesinin kendi değerlerine göre sıralandığını gösterir. Sıfır veya daha büyük olduğunda, veri bölgesindeki veri alanının dizinini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


[SortOrder](../../com.aspose.cells/sortorder) öğesini temsil eder.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

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

