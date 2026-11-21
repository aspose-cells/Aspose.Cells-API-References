---
title: "FormatConditionType"
second_title: "Aspose.Cells för Java API-referens"
description: "Typ av villkorsformateringsregel."
type: docs
url: /sv/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

Typ av villkorsformateringsregel.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | Denna villkorsformateringsregel markerar celler som är över eller under medelvärdet för alla värden i intervallet. |
| [BEGINS_WITH](#BEGINS-WITH) | Denna villkorsformateringsregel markerar celler i intervallet som börjar med den angivna texten. |
| [CELL_VALUE](#CELL-VALUE) | Denna villkorsformateringsregel jämför ett cellvärde med ett formelberäknat resultat med hjälp av en operator. |
| [COLOR_SCALE](#COLOR-SCALE) | Denna villkorsformateringsregel skapar en graderad färgskala på cellerna. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | Denna villkorsformateringsregel markerar celler som är helt tomma. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | Denna villkorsformateringsregel markerar celler med formelfel. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | Denna villkorsformateringsregel markerar celler som innehåller den angivna texten. |
| [DATA_BAR](#DATA-BAR) | Denna villkorsformateringsregel visar en graderad datastapel i cellintervallet. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | Denna villkorsformateringsregel markerar duplicerade värden. |
| [ENDS_WITH](#ENDS-WITH) | Denna villkorsformateringsregel markerar celler som slutar med den angivna texten. |
| [EXPRESSION](#EXPRESSION) | Denna villkorsformateringsregel innehåller en formel att utvärdera. |
| [ICON_SET](#ICON-SET) | Denna villkorsformateringsregel tillämpar ikoner på celler enligt deras värden. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | Denna villkorsformateringsregel markerar celler som inte är tomma. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | Denna villkorsformateringsregel markerar celler utan formelfel. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | Denna villkorsformateringsregel markerar celler som inte innehåller den angivna texten. |
| [TIME_PERIOD](#TIME-PERIOD) | Denna villkorsformateringsregel markerar celler som innehåller datum inom den angivna tidsperioden. |
| [TOP_10](#TOP-10) | Denna villkorsformateringsregel markerar celler vars värden faller i de översta N eller nedersta N intervallen, enligt specifikationen. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | Denna villkorsformateringsregel markerar unika värden i intervallet. |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


Denna villkorsformateringsregel markerar celler som är över eller under medelvärdet för alla värden i intervallet.

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


Denna villkorsformateringsregel markerar celler i intervallet som börjar med den angivna texten. Motsvarande att använda LEFT()-funktion i kalkylbladet och jämföra värden.

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Denna villkorsformateringsregel jämför ett cellvärde med ett formelberäknat resultat med hjälp av en operator.

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


Denna villkorsformateringsregel skapar en graderad färgskala på cellerna.

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


Denna villkorsformateringsregel markerar celler som är helt tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen endast innehåller tecken som TRIM() skulle ta bort, anses den vara tom. En tom cell anses också vara tom.

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


Denna villkorsformateringsregel markerar celler med formelfel. Motsvarande att använda ISERROR()-funktionen i kalkylbladet för att avgöra om det finns ett formelfel.

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


Denna villkorsformateringsregel markerar celler som innehåller den angivna texten. Motsvarande att använda SEARCH()-funktionen i kalkylbladet för att avgöra om cellen innehåller texten.

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


Denna villkorsformateringsregel visar en graderad datastapel i cellintervallet.

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


Denna villkorsformateringsregel markerar duplicerade värden.

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


Denna villkorsformateringsregel markerar celler som slutar med given text. Motsvarande att använda RIGHT()-funktion i kalkylbladet och jämföra värden.

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


Denna villkorsformateringsregel innehåller en formel att utvärdera. När formelresultatet är sant markeras cellen.

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


Denna villkorsformateringsregel tillämpar ikoner på celler enligt deras värden.

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


Denna villkorsformateringsregel markerar celler som inte är tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen bara innehåller tecken som TRIM() skulle ta bort, betraktas den som tom. En tom cell betraktas också som tom.

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


Denna villkorsformateringsregel markerar celler utan formelfel. Motsvarande att använda ISERROR()-funktionen i kalkylbladet för att avgöra om det finns ett formelfel.

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


Denna villkorsformateringsregel markerar celler som inte innehåller given text. Motsvarande att använda SEARCH()-funktionen i kalkylbladet för att avgöra om cellen innehåller texten eller inte.

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


Denna villkorsformateringsregel markerar celler som innehåller datum inom den angivna tidsperioden. Cellens underliggande värde utvärderas, så cellen behöver inte vara formaterad som ett datum för att utvärderas. Till exempel, med en cell som innehåller värdet 38913 ska den villkorliga formateringen tillämpas om regeln kräver värdet 7/14/2006.

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


Denna villkorsformateringsregel markerar celler vars värden faller i de översta N eller nedersta N intervallen, enligt specifikationen.

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


Denna villkorsformateringsregel markerar unika värden i intervallet.

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

