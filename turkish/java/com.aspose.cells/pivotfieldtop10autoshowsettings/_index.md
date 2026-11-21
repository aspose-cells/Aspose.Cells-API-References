---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pivot alanı için En İyi 10 Otomatik Gösterme ayarlarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

Pivot alanı için En İyi 10 Otomatik Gösterme ayarlarını temsil eder.

**Remarks**

xls içinde: Xls'te Top 10 AutoShow aracılığıyla top 10 filtrelerini uygulama ooxml dosyalarında: Temel ooxml dosya formatı Top10 AutoShow'u destekler, ancak Excel 2007 ve sonraki sürümlerin kullanıcı arayüzü yalnızca Top10 filtresi üzerinden erişim sağlar. XLS uyumluluğu gerekli değilse, Top10 filtresinin kullanılması önerilir.

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
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğe sayısını temsil eder. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | AutoShow sıralaması için veri alanının indeksini belirtir. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | Bu alana \"Top 10 AutoShow\" filtresinin uygulanıp uygulanmadığını gösterir. |
| [isTop()](#isTop--) | Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Bu alana \"Top 10 AutoShow\" filtresinin uygulanıp uygulanmadığını gösterir. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğe sayısını temsil eder. |
| [setRankBy(int value)](#setRankBy-int-) | AutoShow sıralaması için veri alanının indeksini belirtir. |
| [setTop(boolean value)](#setTop-boolean-) | Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir. |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğe sayısını temsil eder.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


AutoShow sıralaması için veri alanının dizinini belirtir. Otomatik gösterim alanı dizinini temsil eder. -1, PivotField kendisini ifade eder. Veri alanlarının dizini olmalıdır.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Bu alana \"Top 10 AutoShow\" filtresinin uygulanıp uygulanmadığını gösterir.

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Bu alana \"Top 10 AutoShow\" filtresinin uygulanıp uygulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğe sayısını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


AutoShow sıralaması için veri alanının dizinini belirtir. Otomatik gösterim alanı dizinini temsil eder. -1, PivotField kendisini ifade eder. Veri alanlarının dizini olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir.

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

