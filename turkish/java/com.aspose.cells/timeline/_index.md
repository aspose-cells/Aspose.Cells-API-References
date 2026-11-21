---
title: "Timeline"
second_title: "Aspose.Cells for Java API Referansı"
description: "Timeline Görünümünün özet açıklaması. MS Excel 2003 Timeline'ı desteklemediği için"
type: docs
url: /tr/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

Timeline Görünümü özeti: MS Excel nedeniyle, Excel 2003 Timeline'ı desteklemez.

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
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | Bu Timeline'ın başlığını alır. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | Timeline'ın mevcut zaman seviyesi. |
| [getHeightPixel()](#getHeightPixel--) | Belirtilen timeline'ın yüksekliğini piksel cinsinden döndürür veya ayarlar. |
| [getLeftPixel()](#getLeftPixel--) | Timeline şeklinin sol sütunundan yatay ofsetini piksel cinsinden döndürür veya ayarlar. |
| [getName()](#getName--) | Belirtilen Timeline'ın adını döndürür veya ayarlar. |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | Seçilen tarih saat aralığını alır. |
| [getSelectionLevel()](#getSelectionLevel--) | Timeline için mevcut seçimin yapıldığı zaman seviyesini alır. |
| [getShape()](#getShape--) | Bu Timeline ile ilişkili [TimelineShape](../../com.aspose.cells/timelineshape) nesnesini döndürür. |
| [getShowHeader()](#getShowHeader--) | Bu timeline'ın başlığının gösterilip gösterilmeyeceğini belirtir. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | Yatay kaydırma çubuğunun gösterilip gösterilmeyeceğini belirtir. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | Seçim etiketinin gösterilip gösterilmeyeceğini belirtir. |
| [getShowTimeLevel()](#getShowTimeLevel--) | Zaman seviyesinin açılır seçim kutusunun gösterilip gösterilmeyeceğini belirtir. |
| [getStartDate()](#getStartDate--) | Bu [Timeline](../../com.aspose.cells/timeline) zaman aralığı kaydırma konumunun başlangıç tarihini alır. |
| [getTopPixel()](#getTopPixel--) | Timeline şeklinin üst satırından dikey ofsetini piksel cinsinden döndürür veya ayarlar. |
| [getWidthPixel()](#getWidthPixel--) | Belirtilen timeline'ın genişliğini piksel cinsinden döndürür veya ayarlar. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | Tarih ve saat arasında öğe seçin. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Bu Timeline'ın başlığını ayarlar. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | Timeline'ın mevcut zaman seviyesi. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Belirtilen timeline'ın yüksekliğini piksel cinsinden döndürür veya ayarlar. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Timeline şeklinin sol sütunundan yatay ofsetini piksel cinsinden döndürür veya ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Belirtilen Timeline'ın adını döndürür veya ayarlar. |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | Timeline için mevcut seçimin yapıldığı zaman seviyesini ayarlar. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | Bu timeline'ın başlığının gösterilip gösterilmeyeceğini belirtir. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | Yatay kaydırma çubuğunun gösterilip gösterilmeyeceğini belirtir. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | Seçim etiketinin gösterilip gösterilmeyeceğini belirtir. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | Zaman seviyesinin açılır seçim kutusunun gösterilip gösterilmeyeceğini belirtir. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Bu [Timeline](../../com.aspose.cells/timeline) zaman aralığı kaydırma konumunun başlangıç tarihini ayarlar. |
| [setTopPixel(int value)](#setTopPixel-int-) | Timeline şeklinin üst satırından dikey ofsetini piksel cinsinden döndürür veya ayarlar. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Belirtilen timeline'ın genişliğini piksel cinsinden döndürür veya ayarlar. |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


Bu Timeline'ın başlığını alır.

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


Timeline'ın mevcut zaman seviyesi.

Bak [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Belirtilen timeline'ın yüksekliğini piksel cinsinden döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Height özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Timeline şeklinin sol sütunundan yatay ofsetini piksel cinsinden döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Left özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Belirtilen Timeline'ın adını döndürür veya ayarlar.

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


Seçilen tarih saat aralığını alır.

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


Timeline için mevcut seçimin yapıldığı zaman seviyesini alır.

Bak [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


Bu Timeline ile ilişkili [TimelineShape](../../com.aspose.cells/timelineshape) nesnesini döndürür.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


Bu timeline'ın başlığının gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


Yatay kaydırma çubuğunun gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


Seçim etiketinin gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


Zaman seviyesinin açılır seçim kutusunun gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Bu [Timeline](../../com.aspose.cells/timeline) zaman aralığı kaydırma konumunun başlangıç tarihini alır.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Timeline şeklinin üst satırından dikey ofsetini piksel cinsinden döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Top özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Belirtilen timeline'ın genişliğini piksel cinsinden döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Width özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


Tarih ve saat arasında öğe seçin.

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | Başlangıç tarih ve saat |
| end | [DateTime](../../com.aspose.cells/datetime) | Bitiş tarih ve saat |
| hesapla | boolean | İlgili pivot tablolarının hesaplanıp hesaplanmayacağını gösterir |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Bu Timeline'ın başlığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


Timeline'ın mevcut zaman seviyesi.

Bak [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Belirtilen timeline'ın yüksekliğini piksel cinsinden döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Height özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Timeline şeklinin sol sütunundan yatay ofsetini piksel cinsinden döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Left özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Belirtilen Timeline'ın adını döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


Timeline için mevcut seçimin yapıldığı zaman seviyesini ayarlar.

Bak [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


Bu timeline'ın başlığının gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


Yatay kaydırma çubuğunun gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


Seçim etiketinin gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


Zaman seviyesinin açılır seçim kutusunun gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Bu [Timeline](../../com.aspose.cells/timeline) zaman aralığı kaydırma konumunun başlangıç tarihini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Timeline şeklinin üst satırından dikey ofsetini piksel cinsinden döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Top özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Belirtilen timeline'ın genişliğini piksel cinsinden döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Width özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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

