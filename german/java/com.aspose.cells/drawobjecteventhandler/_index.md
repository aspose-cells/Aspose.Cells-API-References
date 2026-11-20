---
title: "DrawObjectEventHandler"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Schnittstelle zum Abrufen von DrawObject und Bound beim Rendern."
type: docs
url: /de/java/com.aspose.cells/drawobjecteventhandler/
---

**Inheritance:**
java.lang.Object
```
public abstract class DrawObjectEventHandler
```

Schnittstelle zum Abrufen von DrawObject und Bound beim Rendern.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DrawObjectEventHandler()](#DrawObjectEventHandler--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [draw(DrawObject drawObject, float x, float y, float width, float height)](#draw-com.aspose.cells.DrawObject-float-float-float-float-) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
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


Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| drawObject | [DrawObject](../../com.aspose.cells/drawobject) | DrawObject wird beim Rendern initialisiert und zurückgegeben. |
| x | float | Linke Seite von DrawObject |
| y | float | Obere Seite von DrawObject |
| Breite | float | Breite von DrawObject |
| Höhe | float | Höhe von DrawObject |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

