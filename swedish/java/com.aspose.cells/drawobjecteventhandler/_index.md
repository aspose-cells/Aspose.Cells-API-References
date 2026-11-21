---
title: "DrawObjectEventHandler"
second_title: "Aspose.Cells för Java API-referens"
description: "Gränssnitt för att hämta DrawObject och Bound vid rendering."
type: docs
url: /sv/java/com.aspose.cells/drawobjecteventhandler/
---

**Inheritance:**
java.lang.Object
```
public abstract class DrawObjectEventHandler
```

Gränssnitt för att hämta DrawObject och Bound vid rendering.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [DrawObjectEventHandler()](#DrawObjectEventHandler--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [draw(DrawObject drawObject, float x, float y, float width, float height)](#draw-com.aspose.cells.DrawObject-float-float-float-float-) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
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


Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| drawObject | [DrawObject](../../com.aspose.cells/drawobject) | DrawObject kommer att initieras och returneras vid rendering. |
| x | float | Vänster på DrawObject |
| y | float | Toppen av DrawObject |
| bredd | float | Bredd på DrawObject |
| höjd | float | Höjd på DrawObject |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

