---
title: "GridCalculationData"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar den nödvändiga datan när en funktion beräknas, såsom funktionsnamn, parametrar ...etc."
type: docs
url: /sv/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Representerar den nödvändiga data vid beräkning av en funktion, såsom funktionsnamn, parametrar, …etc.

**Remarks**

Alla objekt som tillhandahålls av denna klass är endast avsedda för "läs"-ändamål. Användaren bör inte ändra någon data i Workbook under formelberäkningsprocessen, annars kan oväntade resultat eller undantag uppstå.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Hämtar det beräknade värdet för denna funktion. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hämtar cellens kolumnindex där funktionen finns. |
| [getFormula()](#getFormula--) | Hämtar cellens formel där funktionen finns. |
| [getFunctionName()](#getFunctionName--) | Hämtar funktionsnamnet som ska beräknas. |
| [getParamCount()](#getParamCount--) | Hämtar antalet parametrar. |
| [getParamText(int index)](#getParamText-int-) | Hämtar den bokstavliga texten för parametern på angivet index. |
| [getParamValue(int index)](#getParamValue-int-) | Hämtar det representerade värdeobjektet för parametern på angivet index. |
| [getRow()](#getRow--) | Hämtar cellens radindex där funktionen finns. |
| [getSheetName()](#getSheetName--) | Hämtar arbetsbladets namn där funktionen finns. |
| [getStringValue()](#getStringValue--) | Hämtar cellens DisplayStringValue där funktionen finns. |
| [getValue()](#getValue--) | Hämtar cellens värde där funktionen finns. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Ställer in det beräknade värdet för denna funktion. |
| [toString()](#toString--) |  |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Hämtar det beräknade värdet för denna funktion.

**Remarks**

Användaren bör sätta denna egenskap i sin anpassade beräkningsmotor för de funktioner som motorn stöder, och det satta värdet kommer att returneras när egenskapen hämtas. Att hämta denna egenskap innan den sätts kommer att göra att funktionen beräknas av standardberäkningsmotorn i Aspose.Cells och det beräknade värdet kommer att returneras.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Hämtar cellens kolumnindex där funktionen finns.

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


Hämtar cellens formel där funktionen finns.

**Returns:**
java.lang.String
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


Hämtar funktionsnamnet som ska beräknas.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


Hämtar antalet parametrar.

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Hämtar den bokstavliga texten för parametern på angivet index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet för parametern (0-baserat). |

**Returns:**
java.lang.String - Den bokstavliga texten för parametern.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Hämtar det representerade värdeobjektet för parametern på angivet index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet för parametern (0-baserat). |

**Returns:**
java.lang.Object - Om parametern är ett enkelt värde, returneras det enkla värdet. Om parametern är en referens, returneras ett ReferredArea-objekt.
### getRow() {#getRow--}
```
public int getRow()
```


Hämtar cellens radindex där funktionen finns.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Hämtar arbetsbladets namn där funktionen finns.

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Hämtar cellens DisplayStringValue där funktionen finns.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Hämtar cellens värde där funktionen finns.

**Returns:**
java.lang.Object
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


Ställer in det beräknade värdet för denna funktion.

**Remarks**

Användaren bör sätta denna egenskap i sin anpassade beräkningsmotor för de funktioner som motorn stöder, och det satta värdet kommer att returneras när egenskapen hämtas. Att hämta denna egenskap innan den sätts kommer att göra att funktionen beräknas av standardberäkningsmotorn i Aspose.Cells och det beräknade värdet kommer att returneras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

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

