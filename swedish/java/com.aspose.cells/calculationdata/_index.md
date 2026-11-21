---
title: "CalculationData"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar den nödvändiga datan när en funktion beräknas, såsom funktionsnamn, parametrar ...etc."
type: docs
url: /sv/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

Representerar den nödvändiga data vid beräkning av en funktion, såsom funktionsnamn, parametrar, …etc.

**Remarks**

Alla objekt som tillhandahålls av denna klass är endast avsedda för "läs"-ändamål. Användaren bör inte ändra någon data i Workbook under formelberäkningsprocessen, annars kan oväntade resultat eller undantag uppstå.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Hämtar det beräknade värdet för denna funktion. |
| [getCell()](#getCell--) | Hämtar Cell-objektet där funktionen är. |
| [getCellColumn()](#getCellColumn--) | Hämtar kolumnindexet för cellen där funktionen är. |
| [getCellRow()](#getCellRow--) | Hämtar radindex för cellen där funktionen finns. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Hämtar funktionsnamnet som ska beräknas. |
| [getParamCount()](#getParamCount--) | Hämtar antalet parametrar |
| [getParamText(int index)](#getParamText-int-) | Hämtar den bokstavliga texten för parametern på det angivna indexet. |
| [getParamValue(int index)](#getParamValue-int-) | Hämtar det representerade värdeobjektet för parametern på ett givet index. |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | Hämtar värdet/värdena för parametern på ett givet index. |
| [getWorkbook()](#getWorkbook--) | Hämtar Workbook‑objektet där funktionen finns. |
| [getWorksheet()](#getWorksheet--) | Hämtar Worksheet‑objektet där funktionen finns. |
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

Användaren bör sätta denna egenskap i sin anpassade beräkningsmotor för de funktioner som motorn stödjer, och det satta värdet kommer att returneras när egenskapen hämtas senare. Det satta värdet kan vara av möjliga typer som [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), eller en array av sådana värden, eller ett Range, Name, ReferredArea. Att hämta denna egenskap innan ett värde har satts på den gör att funktionen beräknas av standard‑beräkningsmotorn i Aspose.Cells och sedan returneras det beräknade värdet (vanligtvis bör det vara \#NAME? för användardefinierade funktioner).

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


Hämtar Cell-objektet där funktionen är.

**Remarks**

När en formel beräknas utan att den sätts i en cell, till exempel via [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-), beräknas formeln som om den hade satts i cell A1, så både [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) och [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) är 0. Däremot kan cell A1 i kalkylbladet ha saknat instansiering. Så i en sådan situation blir denna egenskap null.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Hämtar kolumnindexet för cellen där funktionen är.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Hämtar radindex för cellen där funktionen finns.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


Hämtar antalet parametrar

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Hämtar den bokstavliga texten för parametern på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | index för parametern (0‑baserat) |

**Returns:**
java.lang.String – bokstavlig text för parametern
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Hämtar det representerade värdeobjektet för parametern på ett givet index.

**Remarks**

För en parameter:

Om det är ett enkelt värde, returneras själva enkla värdet;

Om det är en referens, returneras ett ReferredArea‑objekt;

Om det refererar till dataset med flera värden, returneras en array av objekt;

Om det är någon form av uttryck som måste beräknas, beräknas det i värdeläge och generellt returneras ett enda värde baserat på den aktuella cellens referens. Till exempel, om en parameter i D2:s formel är A:A+B:B, beräknas och returneras A2+B2. Däremot, om denna parameter har angivits i arrayläge (av  eller ), returneras en array (object[][]) vars element är A1+B1, A2+B2, ….

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Index för parametern (0‑baserat) |

**Returns:**
java.lang.Object – Det beräknade värdet för parametern.
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


Hämtar värdet/värdena för parametern på ett givet index. Om parametern är någon form av uttryck som måste beräknas, beräknas den i arrayläge.

**Remarks**

För ett uttryck som måste beräknas, med A:A+B:B som exempel: I värdeläge beräknas det till ett enda värde baserat på den aktuella cellen. Men i arrayläge beräknas alla värden för A1+B1, A2+B2, A3+B3, … och används för att konstruera den returnerade arrayen. I en sådan situation är det bättre att ange en gräns för rad‑/kolumnantalet (t.ex. enligt [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) och [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--)), annars kan den stora returnerade arrayen öka minneskostnaden med en stor mängd onödig data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Index för parametern (0‑baserat) |
| maxRowCount | int | Radantalgränsen för den returnerade arrayen. Om den är noll eller negativ eller större än det faktiska radantalet, kommer det faktiska radantalet att användas. |
| maxColumnCount | int | Kolumnantalgränsen för den returnerade arrayen. Om den är noll eller negativ eller större än det faktiska radantalet, kommer det faktiska kolumnantalet att användas. |

**Returns:**
java.lang.Object[][] - En array som innehåller alla objekt som representeras av den angivna parametern.
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Hämtar Workbook‑objektet där funktionen finns.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Hämtar Worksheet‑objektet där funktionen finns.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

Användaren bör sätta denna egenskap i sin anpassade beräkningsmotor för de funktioner som motorn stödjer, och det satta värdet kommer att returneras när egenskapen hämtas senare. Det satta värdet kan vara av möjliga typer som [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), eller en array av sådana värden, eller ett Range, Name, ReferredArea. Att hämta denna egenskap innan ett värde har satts på den gör att funktionen beräknas av standard‑beräkningsmotorn i Aspose.Cells och sedan returneras det beräknade värdet (vanligtvis bör det vara \#NAME? för användardefinierade funktioner).

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

