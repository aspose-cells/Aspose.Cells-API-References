---
title: "AccessCacheOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Cache‑alternativ för dataåtkomst."
type: docs
url: /sv/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

Cachealternativ för dataåtkomst. Flera alternativ kan kombineras med "\|"-operatorn.

**Remarks**

För vissa funktioner kräver åtkomst till stora dataset många upprepade och komplicerade operationer såsom sökning, beräkning, …etc och dessa operationer tar mycket extra tid. För vanliga situationer förblir all beroende data oförändrad under åtkomsten, så vissa cachar kan byggas och användas för att förbättra åtkomstprestandan. För detta ändamål tillhandahåller vi detta API så att användaren kan ange vilken typ av dataåtkomst som bör optimeras med en möjlig cachemekanism.

Observera att för olika alternativ kan olika dataset behöva vara "read-only". Och prestandan för dataåtkomst beror på många faktorer; användning av en cachemekanism garanterar inte att prestandan förbättras. I vissa situationer, till exempel när datasetet som ska nås är litet, kan användning av cache ta ännu mer tid eftersom cachning i sig också kräver viss extra tid.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ALL](#ALL) | Tillämpa alla möjliga optimeringar för alla typer av dataåtkomst i arbetsboken. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | Tillämpa möjlig optimering för beräkning av formler. |
| [CELLS_DATA](#CELLS-DATA) | Tillämpa möjlig optimering för hämtning av cellvärden. |
| [CELL_DISPLAY](#CELL-DISPLAY) | Tillämpa möjlig optimering för att hämta displayrelaterade resultat för celler([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Tillämpa möjlig optimering för att hämta formateringsresultat för villkorliga formateringar. |
| [GET_FORMULA](#GET-FORMULA) | Tillämpa möjlig optimering för att hämta formler. |
| [NONE](#NONE) | Ingen cache för någon dataåtkomst. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | Tillämpa möjlig optimering för att hämta ett objekts (t.ex. Shape) position och storlek. |
| [SET_FORMULA](#SET-FORMULA) | Tillämpa möjlig optimering för att sätta formler. |
| [VALIDATION](#VALIDATION) | Tillämpa möjlig optimering för att hämta valideringsresultat. |
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
### ALL {#ALL}
```
public static final int ALL
```


Tillämpa alla möjliga optimeringar för alla typer av dataåtkomst i arbetsboken. Alla inställningar och data får inte ändras under den optimerade åtkomsten.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


Tillämpa möjlig optimering för beräkning av formler. Celldata får inte ändras under den optimerade åtkomsten, och inga nya objekt (Cell, Row, etc.) får skapas heller (t.ex. via [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


Tillämpa möjlig optimering för att hämta cellers värden. Celldata (data och inställningar för Cell, Row) bör inte ändras under den optimerade åtkomsten, och inga nya Cell/Row‑objekt bör skapas heller (t.ex. via [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


Tillämpa möjlig optimering för att hämta displayrelaterade resultat för celler ([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). Celldata och stilrelaterade objekt (Cell/Row/Column‑stilar, kolumnbredd, etc.) bör inte ändras under den optimerade åtkomsten.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Tillämpa möjlig optimering för att hämta formateringsresultat för villkorsformatering. All data och alla inställningar som kan påverka resultatet av villkorsformatering (inställningar för villkorsformatering, beroende cellvärden, etc.) bör inte ändras under den optimerade åtkomsten.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


Tillämpa möjlig optimering för att hämta formler. All data och alla inställningar som kan påverka formeluttrycket (arbetsbladets namn, namnens text, tabellens kolumn, etc.) bör inte ändras under den optimerade åtkomsten.

### NONE {#NONE}
```
public static final int NONE
```


Ingen cache för någon dataåtkomst.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


Tillämpa möjlig optimering för att hämta ett objekts (t.ex. Shapes) position och storlek. Inställningar för radhöjd och kolumnbredd bör inte ändras under den optimerade åtkomsten.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


Tillämpa möjlig optimering för att sätta formler. All data och alla inställningar som kan påverka formeluttrycket (arbetsbladets namn, namnens text, tabellens kolumn, etc.) bör inte ändras under den optimerade åtkomsten.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Tillämpa möjlig optimering för att hämta valideringsresultat. All data och alla inställningar som kan påverka valideringsresultatet (inställningar för valideringen, beroende cellvärden, etc.) bör inte ändras under den optimerade åtkomsten.

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

