---
title: "SetBorderPosition"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir hücre aralığının ayarlanacak kenar konumunu temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/setborderposition/
---

**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```

Bir hücre aralığının ayarlanacak kenar konumunu temsil eder.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [BOTTOM](#BOTTOM) | Alt kenar |
| [CROSS](#CROSS) | Çapraz kenarlar |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | Alt kenar |
| [LEFT](#LEFT) | Sol kenar |
| [NONE](#NONE) | Kenarlık yok |
| [OUTLINE](#OUTLINE) | DikeyOrta kenarlar |
| [RIGHT](#RIGHT) | Sağ kenar |
| [TOP](#TOP) | Üst kenar |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | YatayOrta kenarlar |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BOTTOM {#BOTTOM}
```
public static final int BOTTOM
```


Alt kenar

### CROSS {#CROSS}
```
public static final int CROSS
```


Çapraz kenarlar

### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```


Alt kenar

### LEFT {#LEFT}
```
public static final int LEFT
```


Sol kenar

### NONE {#NONE}
```
public static final int NONE
```


Kenarlık yok

### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```


DikeyOrta kenarlar

### RIGHT {#RIGHT}
```
public static final int RIGHT
```


Sağ kenar

### TOP {#TOP}
```
public static final int TOP
```


Üst kenar

### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```


YatayOrta kenarlar

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

