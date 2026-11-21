---
title: "IconSet"
second_title: "Aspose.Cells for Java API Referansı"
description: "IconSet koşullu biçimlendirme kuralını açıklar."
type: docs
url: /tr/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

IconSet koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, hücrelere değerlerine göre simgeler uygular.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Icon Set
         IconSet iconSet = cond.getIconSet();
 
         //Set Icon Type
         iconSet.setType(IconSetType.ARROWS_3);
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | Koleksiyondan[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) alın |
| [getCfvos()](#getCfvos--) | CFValueObjects örneğini alın. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | Bu simge setindeki simgelerin varsayılan sırasını tersine çevirip çevirmediğini gösteren bayrağı alır. |
| [getShowValue()](#getShowValue--) | Bu simge setinin uygulandığı hücrelerin değerlerini gösterip göstermediğini belirten bayrağı alır. |
| [getType()](#getType--) | Görüntülenecek simge seti türünü alır. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | Simge setinin özel olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | Bu simge setindeki simgelerin varsayılan sırasını tersine çevirip çevirmediğini gösteren bayrağı ayarlar. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Bu simge setinin uygulandığı hücrelerin değerlerini gösterip göstermediğini belirten bayrağı ayarlar. |
| [setType(int value)](#setType-int-) | Görüntülenecek simge seti türünü ayarlar. |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


Koleksiyondan[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) alın

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


CFValueObjects örneğini alın.

**Returns:**
[ConditionalFormattingValueCollection](../../com.aspose.cells/conditionalformattingvaluecollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getReverse() {#getReverse--}
```
public boolean getReverse()
```


Bu simge setindeki simgelerin varsayılan sırasını tersine çevirip çevirmediğini gösteren bayrağı alır. Varsayılan değer false.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Bu simge setinin uygulandığı hücrelerin değerlerini gösterip göstermediğini belirten bayrağı alır. Varsayılan değer true.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Görüntülenecek simge seti türünü alır. Tür ayarlandığında, mevcut Cfvos sayısının yeni türle uyumlu olup olmadığı otomatik olarak kontrol edilir. Uyumsuzsa, eski Cfvos temizlenir ve varsayılan Cfvos eklenir.

Bakınız [IconSetType](../../com.aspose.cells/iconsettype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCustom() {#isCustom--}
```
public boolean isCustom()
```


Simge setinin özel olup olmadığını gösterir. Varsayılan değer false.

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




### setReverse(boolean value) {#setReverse-boolean-}
```
public void setReverse(boolean value)
```


Bu simge setindeki simgelerin varsayılan sırasını tersine çevirip çevirmediğini gösteren bayrağı ayarlar. Varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Bu simge setinin uygulandığı hücrelerin değerlerini gösterip göstermediğini belirten bayrağı ayarlar. Varsayılan değer true.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Görüntülenecek simge seti tipini ayarlar. Tipi ayarlamak, mevcut Cfvos sayısının yeni tip ile uyumlu olup olmadığını otomatik olarak kontrol eder. Uyumsuzsa, eski Cfvos temizlenir ve varsayılan Cfvos eklenir.

Bakınız [IconSetType](../../com.aspose.cells/iconsettype).

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

