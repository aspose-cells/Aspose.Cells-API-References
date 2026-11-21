---
title: "AbstractLowCodeProtectionProvider"
second_title: "Aspose.Cells för Java API-referens"
description: "Implementering för att tillhandahålla skyddsinställningar."
type: docs
url: /sv/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

Implementering för att tillhandahålla skyddsinställningar.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | Hämtar lösenordet för att öppna kalkylbladsfilen. |
| [getWorkbookPassword()](#getWorkbookPassword--) | Hämtar lösenordet för att skydda arbetsboken med angiven skyddstyp. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | Hämtar skyddstypen för att skydda arbetsboken. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | Hämtar lösenordet för att skydda det angivna kalkylbladet. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | Hämtar skyddstypen för att skydda det angivna kalkylbladet. |
| [getWritePassword()](#getWritePassword--) | Hämtar lösenordet för att ändra kalkylbladsfilen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
```


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
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```


Hämtar lösenordet för att öppna kalkylbladsfilen.

**Returns:**
java.lang.String - Lösenord för att öppna kalkylbladsfilen. Tomt betyder att det inte finns något skydd för att öppna filen.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


Hämtar lösenordet för att skydda arbetsboken med angiven skyddstyp.

**Returns:**
java.lang.String - Lösenord för att skydda arbetsboken.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


Hämtar skyddstypen för att skydda arbetsboken.

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Skyddstyp för att skydda arbetsboken. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) betyder att det inte finns något skydd för arbetsboken.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


Hämtar lösenordet för att skydda det angivna kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - Lösenord för att skydda det angivna kalkylbladet.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


Hämtar skyddstypen för att skydda det angivna kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Skyddstyp för att skydda det angivna kalkylbladet. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) betyder att det inte finns något skydd för kalkylbladet.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


Hämtar lösenordet för att ändra kalkylbladsfilen.

**Returns:**
java.lang.String - Lösenord för att ändra kalkylbladsfilen. Tomt betyder att det inte finns något skydd för att ändra filen.
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

