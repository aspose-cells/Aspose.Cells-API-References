---
title: "ChartDataTable"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir grafik veri tablosunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

Bir grafik veri tablosunu temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         chart.setShowDataTable(true);
 
         //Getting Chart Table
         ChartDataTable chartTable = chart.getChartDataTable();
 
         //Setting Chart Table Font Color
         chartTable.getFont().setColor(com.aspose.cells.Color.getRed());
 
         //Setting Legend Key VisibilityOptions
         chartTable.setShowLegendKey(false);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [getBackgroundMode()](#getBackgroundMode--) | Arka planın görüntüleme modunu alır |
| [getBorder()](#getBorder--) | Nesnenin kenarını temsil eden bir Border nesnesi döndürür. |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Belirtilen grafik veri tablosunun yazı tipi ayarını temsil eden bir [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) nesnesi alır. |
| [getShowLegendKey()](#getShowLegendKey--) | Veri etiketi açıklama anahtarı görünürse doğru. |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | Grafik veri tablosunda yatay hücre kenarları varsa doğru. |
| [hasBorderOutline()](#hasBorderOutline--) | Grafik veri tablosunda dış kenarlar varsa doğru. |
| [hasBorderVertical()](#hasBorderVertical--) | Grafik veri tablosunda dikey hücre kenarları varsa doğru. |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | Grafik veri tablosunda yatay hücre kenarları varsa doğru. |
| [hasOutlineBorder()](#hasOutlineBorder--) | Grafik veri tablosunda dış kenarlar varsa doğru. |
| [hasVerticalBorder()](#hasVerticalBorder--) | Grafik veri tablosunda dikey hücre kenarları varsa doğru. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Arka planın görüntüleme modunu ayarlar |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | Grafik veri tablosunda yatay hücre kenarları varsa doğru. |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | Grafik veri tablosunda dış kenarlar varsa doğru. |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | Grafik veri tablosunda dikey hücre kenarları varsa doğru. |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | Grafik veri tablosunda yatay hücre kenarları varsa doğru. |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | Grafik veri tablosunda dış kenarlar varsa doğru. |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | Grafik veri tablosunda dikey hücre kenarları varsa doğru. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Veri etiketi açıklama anahtarı görünürse doğru. |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. Varsayılan değer Doğru.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Arka planın görüntüleme modunu alır

Bakınız [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Nesnenin kenarını temsil eden bir Border nesnesi döndürür.

**Returns:**
[Line](../../com.aspose.cells/line)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


Belirtilen grafik veri tablosunun yazı tipi ayarını temsil eden bir [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) nesnesi alır.

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Veri etiketi açıklama anahtarı görünürse doğru.

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


Grafik veri tablosunda yatay hücre kenarları varsa doğru.

**Remarks**

NOTE: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen ChartDataTable.HasHorizontalBorder özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


Grafik veri tablosunda dış kenarlar varsa doğru.

**Remarks**

NOTE: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen ChartDataTable.HasOutlineBorder özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


Grafik veri tablosunda dikey hücre kenarları varsa doğru.

**Remarks**

NOTE: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen ChartDataTable.HasVerticalBorder özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


Grafik veri tablosunda yatay hücre kenarları varsa doğru.

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


Grafik veri tablosunda dış kenarlar varsa doğru.

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


Grafik veri tablosunda dikey hücre kenarları varsa doğru.

**Returns:**
boolean
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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa doğru. Varsayılan değer Doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Arka planın görüntüleme modunu ayarlar

Bakınız [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


Grafik veri tablosunda yatay hücre kenarları varsa doğru.

**Remarks**

NOTE: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen ChartDataTable.HasHorizontalBorder özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


Grafik veri tablosunda dış kenarlar varsa doğru.

**Remarks**

NOTE: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen ChartDataTable.HasOutlineBorder özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


Grafik veri tablosunda dikey hücre kenarları varsa doğru.

**Remarks**

NOTE: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen ChartDataTable.HasVerticalBorder özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


Grafik veri tablosunda yatay hücre kenarları varsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


Grafik veri tablosunda dış kenarlar varsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


Grafik veri tablosunda dikey hücre kenarları varsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Veri etiketi açıklama anahtarı görünürse doğru.

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

