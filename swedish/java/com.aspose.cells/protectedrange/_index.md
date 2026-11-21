---
title: "ProtectedRange"
second_title: "Aspose.Cells för Java API-referens"
description: "Ett specificerat område som får redigeras när bladskyddet är AKTIVT."
type: docs
url: /sv/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

Ett specificerat område som får redigeras när bladskyddet är AKTIVT.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | Lägger till ett refererat område till detta |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Hämtar alla refererade områden. |
| [getCellArea()](#getCellArea--) | Hämtar [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) objektet som representerar det cellområde som ska skyddas. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Hämtar områdets titel. |
| [getPassword()](#getPassword--) | Representerar lösenordet för att skydda området. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | Säkerhetsbeskrivningen definierar användarkonton som kan redigera detta område utan att ange ett lösenord för att komma åt området. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Anger om kalkylbladet är skyddat med lösenord. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | Hämtar områdets titel. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Representerar lösenordet för att skydda området. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | Säkerhetsbeskrivningen definierar användarkonton som kan redigera detta område utan att ange ett lösenord för att komma åt området. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


Lägger till ett refererat område till detta

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startrad. |
| startColumn | int | Startkolumnen. |
| slutRad | int | Slutrad. |
| endColumn | int | Slutkolumn. |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Hämtar alla refererade områden.

**Returns:**
com.aspose.cells.CellArea[] - Returnerar alla refererade områden.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Hämtar [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) objektet som representerar det cellområde som ska skyddas.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Hämtar områdets titel. Detta används som en beskrivning, inte som en namngiven områdesdefinition.

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


Representerar lösenordet för att skydda området.

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


Säkerhetsbeskrivningen definierar användarkonton som kan redigera detta område utan att ange ett lösenord för att komma åt området.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Anger om kalkylbladet är skyddat med lösenord.

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




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Hämtar områdets titel. Detta används som en beskrivning, inte som en namngiven områdesdefinition.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Representerar lösenordet för att skydda området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


Säkerhetsbeskrivningen definierar användarkonton som kan redigera detta område utan att ange ett lösenord för att komma åt området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

