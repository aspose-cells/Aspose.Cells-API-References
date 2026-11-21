---
title: "GridShape"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir şekil nesnesini temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

Bir şekil nesnesini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | Nesnenin tamponunu alır. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | Şekil için Set ID'sini alır. |
| [getLeft()](#getLeft--) | Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder. |
| [getLeftToCorner()](#getLeftToCorner--) | Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde temsil eder. |
| [getMsoDrawingType()](#getMsoDrawingType--) | mso çizim tipini alır. |
| [getName()](#getName--) | Şeklin adını alır. |
| [getText()](#getText--) | Bu TextBox nesnesindeki dizeyi temsil eder. |
| [getTop()](#getTop--) | Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder. |
| [getTopToCorner()](#getTopToCorner--) | Şeklin çalışma sayfasının üst kenarından dikey ofsetini, piksel biriminde temsil eder. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Sol üst köşe sütun indeksini temsil eder. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Üst sol köşe satır indeksini temsil eder. |
| [getZOrderPosition()](#getZOrderPosition--) | Bir şeklin z-sırasındaki konumunu döndürür. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Görüntüyü oluşturur ve belirtilen png formatında bir akışa kaydeder. |
| [setID(String value)](#setID-java.lang.String-) | Şekil için Set ID'sini alır. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde temsil eder. |
| [setText(String value)](#setText-java.lang.String-) | Bu TextBox nesnesindeki dizeyi temsil eder. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Şeklin çalışma sayfasının üst kenarından dikey ofsetini, piksel biriminde temsil eder. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Bir şeklin z-sırasındaki konumunu döndürür. |
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
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


Nesnenin tamponunu alır.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getID() {#getID--}
```
public String getID()
```


Şekil için Set ID'sini alır.

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


Şeklin sol sütunundan yatay kaymasını, piksel biriminde temsil eder.

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde temsil eder.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


mso çizim tipini alır.

Bak [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Şeklin adını alır.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Bu TextBox nesnesindeki dizeyi temsil eder.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Şeklin üst satırından dikey ofsetini, piksel biriminde temsil eder.

**Remarks**

Şekil grafikte ise, şeklin üst kenarından dikey ofsetini temsil eder.

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Şeklin çalışma sayfasının üst kenarından dikey ofsetini, piksel biriminde temsil eder.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Sol üst köşe sütun indeksini temsil eder.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Üst sol köşe satır indeksini temsil eder.

**Remarks**

Şekil bir şekil içinde veya bir grup içinde ise, UpperLeftRow yoksayılacaktır.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Bir şeklin z-sırasındaki konumunu döndürür.

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




### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Görüntüyü oluşturur ve belirtilen png formatında bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Şekil için Set ID'sini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Şeklin çalışma sayfasının sol kenarından yatay ofsetini, piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Bu TextBox nesnesindeki dizeyi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Şeklin çalışma sayfasının üst kenarından dikey ofsetini, piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Bir şeklin z-sırasındaki konumunu döndürür.

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

