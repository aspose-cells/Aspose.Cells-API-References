---
title: "TxtValueQuoteType"
second_title: "Aspose.Cells för Java API-referens"
description: "Anger typen av användning av citattecken för värden i textformatfiler."
type: docs
url: /sv/java/com.aspose.cells/txtvaluequotetype/
---

**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```

Anger typen av användning av citattecken för värden i textformatfiler.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ALWAYS](#ALWAYS) | Alla värden kommer alltid att omges av citationstecken. |
| [MINIMUM](#MINIMUM) | Omge bara värden med citationstecken när det behövs. |
| [NEVER](#NEVER) | Alla värden kommer inte att omges av citationstecken. |
| [NORMAL](#NORMAL) | Alla värden som innehåller specialtecken såsom citattecken eller avgränsningstecken kommer att omges av citationstecken. |
## Metoder

| Metod | Beskrivning |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Alla värden kommer alltid att omges av citationstecken.

### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```


Omge bara värden med citationstecken när det behövs. Till exempel, om ett värde innehåller ett citattecken men citattecknet inte är i början av värdet, kommer detta värde inte att omges av citationstecken.

### NEVER {#NEVER}
```
public static final int NEVER
```


Alla värden kommer inte att omges av citationstecken. Den exporterade textfilen av den här typen kanske inte kan läsas korrekt tillbaka eftersom nödvändiga citationstecken saknas.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Alla värden som innehåller specialtecken såsom citattecken eller avgränsningstecken kommer att omges av citationstecken. Samma beteende som i MS Excel vid export av textfil.

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

