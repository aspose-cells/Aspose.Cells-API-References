---
title: "Column"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma sayfasındaki tek bir sütunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

Bir çalışma sayfasındaki tek bir sütunu temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Get first Column
         Column column = worksheet.getCells().getColumns().get(0);
 
         //Apply Style to first Column
         column.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tüm bir sütun için biçimleri uygular. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Sütunun grup seviyesini alır. |
| [getIndex()](#getIndex--) | Bu sütunun dizinini alır. |
| [getStyle()](#getStyle--) | Bu sütunun stilini alır. |
| [getWidth()](#getWidth--) | Sütun genişliğini karakter biriminde alır. |
| [hasCustomStyle()](#hasCustomStyle--) | Bu sütunun özel stil ayarlarına sahip olup olmadığını gösterir (çalışma kitabından devralınan varsayılan stilden farklı). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | sütunun daraltılıp daraltılmadığı |
| [isHidden()](#isHidden--) | Sütunun gizli olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | sütunun daraltılıp daraltılmadığı |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Sütunun grup seviyesini alır. |
| [setHidden(boolean value)](#setHidden-boolean-) | Sütunun gizli olup olmadığını gösterir. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Bu sütunun stilini ayarlar. |
| [setWidth(double value)](#setWidth-double-) | Sütun genişliğini karakter biriminde ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tüm bir sütun için biçimleri uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Uygulanacak stil nesnesi. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

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
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Sütunun grup seviyesini alır.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


Bu sütunun dizinini alır.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Bu sütunun stilini alır.

**Remarks**

Dönen stil nesnesini doğrudan değiştirmek bu sütun veya bu sütundaki hücreler için hiçbir etki yapmaz. Değişikliği bu sütuna uygulamak için [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) veya [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) metodunu çağırmanız gerekir.

Column'un stili, bu sütundaki hücreler tarafından devralınacak stildir (özel stil ayarı olmayan hücreler, örneğin stil açıkça ayarlanmamış mevcut hücreler veya henüz oluşturulmamış hücreler).

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


Sütun genişliğini karakter biriminde alır.

**Remarks**

Elektronik tablo için, sütun genişliği, normal stilin yazı tipinde 0~9 sayılarının en geniş rakamının karakter sayısı olarak ölçülür.

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Bu sütunun özel stil ayarlarına sahip olup olmadığını gösterir (çalışma kitabından devralınan varsayılan stilden farklı).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


sütunun daraltılıp daraltılmadığı

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Sütunun gizli olup olmadığını gösterir.

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




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


sütunun daraltılıp daraltılmadığı

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Sütunun grup seviyesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Sütunun gizli olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Bu sütunun stilini ayarlar.

**Remarks**

Bu yöntem yalnızca verilen stili bu sütun için varsayılan stil olarak ayarlar, bu sütundaki mevcut hücrelerin stil ayarlarını değiştirmez. Mevcut hücrelerin stil ayarlarını aynı anda belirtilen stile güncellemek için lütfen [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\\#applyStyle-Style-StyleFlag-) adresini kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Bu sütundaki hücreler için varsayılan stil olarak kullanılacak stil. |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Sütun genişliğini karakter biriminde ayarlar.

**Remarks**

Elektronik tablo için, sütun genişliği, normal stilin yazı tipinde 0~9 sayılarının en geniş rakamının karakter sayısı olarak ölçülür.

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

