---
title: "DrawObjectEventHandler"
second_title: "Aspose.Cells for Java API Referansı"
description: "İşleme sırasında DrawObject ve Bound almak için arayüz."
type: docs
url: /tr/java/com.aspose.cells/drawobjecteventhandler/
---

**Inheritance:**
java.lang.Object
```
public abstract class DrawObjectEventHandler
```

İşleme sırasında DrawObject ve Bound almak için arayüz.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DrawObjectEventHandler()](#DrawObjectEventHandler--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [draw(DrawObject drawObject, float x, float y, float width, float height)](#draw-com.aspose.cells.DrawObject-float-float-float-float-) | Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DrawObjectEventHandler() {#DrawObjectEventHandler--}
```
public DrawObjectEventHandler()
```


### draw(DrawObject drawObject, float x, float y, float width, float height) {#draw-com.aspose.cells.DrawObject-float-float-float-float-}
```
public void draw(DrawObject drawObject, float x, float y, float width, float height)
```


Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| drawObject | [DrawObject](../../com.aspose.cells/drawobject) | Render işlemi sırasında DrawObject başlatılacak ve döndürülecektir. |
| x | float | DrawObject'in solu |
| y | float | DrawObject'in üstü |
| genişlik | float | DrawObject'in genişliği |
| yükseklik | float | DrawObject'in yüksekliği |

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

