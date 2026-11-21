---
title: "ListColumn"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir Tablo'da sütunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

Bir Tablo'da sütunu temsil eder.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         ListColumn listColumn = table.getListColumns().get(4);
         listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         listColumn.setFormula("=[A]");
         workbook.save("Book1.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | Bu liste sütununun formülünü alır. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | Bu liste sütununun toplam satırının formülünü alır. |
| [getDataStyle()](#getDataStyle--) | Tablodaki bu sütundaki verinin stilini alır. |
| [getFormula()](#getFormula--) | Liste sütununun formülünü alır. |
| [getName()](#getName--) | Sütunun adını alır. |
| [getRange()](#getRange--) | Bu liste sütununun aralığını alır. |
| [getTotalsCalculation()](#getTotalsCalculation--) | Liste sütununun Toplamlar satırındaki hesaplama türünü alır. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | Toplam satırının görüntüleme etiketlerini alır. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | Formülün dizi formülü olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | Bu liste sütunu için formülü ayarlar. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | Bu liste sütununun toplam satırının formülünü alır. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | Tablonun bu sütunundaki verinin stilini ayarlar. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Liste sütununun formülünü ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Sütunun adını ayarlar. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | Liste sütununun Toplamlar satırındaki hesaplama türünü ayarlar. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | Toplam satırının görüntüleme etiketlerini ayarlar. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```


Bu liste sütununun formülünü alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - Bu liste sütununun formülü.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


Bu liste sütununun toplam satırının formülünü alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - Bu liste sütununun formülü.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


Tablodaki bu sütundaki verinin stilini alır.

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Liste sütununun formülünü alır.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Sütunun adını alır.

**Remarks**

Eğer sütunun adı ayarlanırsa, ilgili hücrenin değeri de değişecektir.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Bu liste sütununun aralığını alır.

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


Liste sütununun Toplamlar satırındaki hesaplama türünü alır.

Bakın [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


Toplam satırının görüntüleme etiketlerini alır.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Formülün dizi formülü olup olmadığını gösterir.

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




### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```


Bu liste sütunu için formülü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Bu liste sütunu için formül. |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


Bu liste sütununun toplam satırının formülünü alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Bu liste sütunu için formül. |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


Tablonun bu sütunundaki verinin stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Liste sütununun formülünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Sütunun adını ayarlar.

**Remarks**

Eğer sütunun adı ayarlanırsa, ilgili hücrenin değeri de değişecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


Liste sütununun Toplamlar satırındaki hesaplama türünü ayarlar.

Bakın [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


Toplam satırının görüntüleme etiketlerini ayarlar.

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

