---
title: "ReferredArea"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett refererat område enligt formeln."
type: docs
url: /sv/java/com.aspose.cells/referredarea/
---

**Inheritance:**
java.lang.Object
```
public class ReferredArea
```

Representerar ett refererat område enligt formeln.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Slutkolumnen för området. |
| [getEndRow()](#getEndRow--) | Slutraden för området. |
| [getExternalFileName()](#getExternalFileName--) | Hämta det externa filnamnet om detta är en extern referens. |
| [getSheetName()](#getSheetName--) | Anger vilket blad den här referensen finns i. |
| [getSheetNames()](#getSheetNames--) | Namn på alla kalkylblad som den här instansen refererar till. |
| [getStartColumn()](#getStartColumn--) | Startkolumnen för området. |
| [getStartRow()](#getStartRow--) | Startraden för området. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Hämtar cellvärde med given offset från övre vänstra hörnet av detta område. |
| [getValue(int rowOffset, int colOffset, boolean calculateFormulas)](#getValue-int-int-boolean-) | Hämtar cellvärde med given offset från övre vänstra hörnet av detta område. |
| [getValues()](#getValues--) | Hämtar cellvärden i detta område. |
| [getValues(boolean calculateFormulas)](#getValues-boolean-) | Hämtar cellvärden i detta område. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Anger om detta är ett område. |
| [isEntireColumn()](#isEntireColumn--) | Anger om detta område innehåller alla rader (hela kolumnen). |
| [isEntireRow()](#isEntireRow--) | Anger om detta område innehåller alla kolumner (hela raden). |
| [isExternalLink()](#isExternalLink--) | Anger om detta är en extern länk. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Returnerar referensadressen för detta område. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Slutkolumnen för området.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Slutraden för området.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


Hämta det externa filnamnet om detta är en extern referens.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Anger vilket blad den här referensen finns i.

**Remarks**

Om den refererar till flera kalkylblad är det returnerade värdet precis som områdesuttrycket i formeln. Till exempel "Sheet1:Sheet3" för referensen i formeln "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

**Returns:**
java.lang.String
### getSheetNames() {#getSheetNames--}
```
public String[] getSheetNames()
```


Namn på alla kalkylblad som den här instansen refererar till.

**Returns:**
java.lang.String[]
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Startkolumnen för området.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Startraden för området.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


Hämtar cellvärde med given offset från övre vänstra hörnet av detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | radoffset från startraden för detta område |
| colOffset | int | kolumnoffset från startraden för detta område |

**Returns:**
java.lang.Object - "\#REF!" om detta område är ogiltigt; "\#N/A" om angivet offset ligger utanför detta område; annars returneras cellvärdet på den angivna positionen.
### getValue(int rowOffset, int colOffset, boolean calculateFormulas) {#getValue-int-int-boolean-}
```
public Object getValue(int rowOffset, int colOffset, boolean calculateFormulas)
```


Hämtar cellvärde med given offset från övre vänstra hörnet av detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | radoffset från startraden för detta område |
| colOffset | int | kolumnoffset från startraden för detta område |
| calculateFormulas | boolean | Om den ska beräknas rekursivt om den angivna referensen är en formel |

**Returns:**
java.lang.Object - "\#REF!" om detta område är ogiltigt; "\#N/A" om angivet offset ligger utanför detta område; annars returneras cellvärdet på den angivna positionen.
### getValues() {#getValues--}
```
public Object getValues()
```


Hämtar cellvärden i detta område.

**Returns:**
java.lang.Object - Om detta område är ogiltigt returneras "\#REF!"; Om detta område är en enda cell returneras cellvärdesobjektet; annars returneras en 2D-array med alla värden i detta område.
### getValues(boolean calculateFormulas) {#getValues-boolean-}
```
public Object getValues(boolean calculateFormulas)
```


Hämtar cellvärden i detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| calculateFormulas | boolean | I detta intervall, om det finns några formler som inte har beräknats, anger denna flagga om dessa formler ska beräknas rekursivt |

**Returns:**
java.lang.Object - Om detta område är ogiltigt returneras "\#REF!"; Om detta område är en enda cell returneras cellvärdesobjektet; annars returneras en 2D-array med alla värden i detta område.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


Anger om detta är ett område.

**Remarks**

Om detta inte är ett område påverkas endast StartRow och StartColumn.

**Returns:**
boolean
### isEntireColumn() {#isEntireColumn--}
```
public boolean isEntireColumn()
```


Anger om detta område innehåller alla rader (hela kolumnen).

**Returns:**
boolean
### isEntireRow() {#isEntireRow--}
```
public boolean isEntireRow()
```


Anger om detta område innehåller alla kolumner (hela raden).

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


Anger om detta är en extern länk.

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




### toString() {#toString--}
```
public String toString()
```


Returnerar referensadressen för detta område. Vanligtvis är det adressen för referensen som kan användas i en formel, till exempel "Sheet1!A1:C3".

**Returns:**
java.lang.String - referensadressen för detta område.
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

