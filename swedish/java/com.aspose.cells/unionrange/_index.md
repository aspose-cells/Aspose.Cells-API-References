---
title: "UnionRange"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar förenad intervall."
type: docs
url: /sv/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

Representerar förenad intervall.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tillämpar format för ett helt område. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | Kopierar området med specialklistra‑alternativ. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | Hämtar antalet celler i intervallet. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Hämtar antalet rader i området. |
| [getFirstColumn()](#getFirstColumn--) | Hämtar indexet för den första kolumnen i området. |
| [getFirstRow()](#getFirstRow--) | Hämtar indexet för den första raden i området. |
| [getHyperlinks()](#getHyperlinks--) | Hämtar alla hyperlänkar i området. |
| [getName()](#getName--) | Hämtar namnet på området. |
| [getRangeCount()](#getRangeCount--) | Hämtar antalet intervall. |
| [getRanges()](#getRanges--) | Hämtar alla förenade intervall. |
| [getRefersTo()](#getRefersTo--) | Hämtar vad området refererar till. |
| [getRowCount()](#getRowCount--) | Hämtar antalet rader i området. |
| [getValue()](#getValue--) | Hämtar värdena i intervallet. |
| [hasRange()](#hasRange--) | Anger om detta har ett intervall. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | Skär med ett annat intervall. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | Skär med ett annat intervall. |
| [intersect(String range)](#intersect-java.lang.String-) | Skär med ett annat intervall. |
| [iterator()](#iterator--) | Hämtar enumeratorn för celler i detta område. |
| [merge()](#merge--) | Kombinerar ett område av celler till en enda cell. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Sätter ett värde i området, om lämpligt kommer värdet att konverteras till en annan datatyp och cellens talformat återställas. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på området. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Ställer in konturkantlinjer runt ett område av celler med samma kantstil och färg. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Ställer in konturkantlinjer runt ett område av celler. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Ställer in stilen för området. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Ställer in värdena i intervallet. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | Ta bort sammanslagning av sammanslagna celler i detta område. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | Förena intervallen. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | Förena ett annat intervall. |
| [union(String range)](#union-java.lang.String-) | Förena ett annat intervall. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tillämpar format för ett helt område.

**Remarks**

Varje cell i detta område kommer att innehålla ett [Style](../../com.aspose.cells/style)-objekt. Så detta är en minneskrävande metod. Använd den med försiktighet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Stilobjektet som kommer att tillämpas. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggor som indikerar tillämpade formateringsegenskaper. |

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


Kopierar området med specialklistra‑alternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | Källintervallet. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Klistra in specialalternativ. |

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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


Hämtar antalet celler i intervallet.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Hämtar antalet rader i området.

**Remarks**

Påverkar endast när det bara innehåller ett intervall.

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Hämtar indexet för den första kolumnen i området.

**Remarks**

Påverkar endast när det bara innehåller ett intervall.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Hämtar indexet för den första raden i området.

**Remarks**

Påverkar endast när det bara innehåller ett intervall.

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Hämtar alla hyperlänkar i området.

**Returns:**
com.aspose.cells.Hyperlink[]
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på området.

**Remarks**

Namngivet område stöds. Till exempel,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Hämtar antalet intervall.

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Hämtar alla förenade intervall.

**Returns:**
com.aspose.cells.Range[]
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Hämtar vad området refererar till.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Hämtar antalet rader i området.

**Remarks**

Påverkar endast när det bara innehåller ett intervall.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Hämtar värdena i intervallet.

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


Anger om detta har ett intervall.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


Skär med ett annat intervall.

**Remarks**

Om de två förenade intervallen inte skär varandra, returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Intervallet. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


Skär med ett annat intervall.

**Remarks**

Om de två förenade intervallen inte skär varandra, returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | Intervallet. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


Skär med ett annat intervall.

**Remarks**

Om de två förenade intervallen inte skär varandra, returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intervall | java.lang.String | Intervallet. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämtar enumeratorn för celler i detta område.

**Remarks**

När element traverseras med den returnerade Enumerator bör cellsamlingen inte modifieras (såsom operationer som skapar nya Cell/Row eller tar bort befintliga Cell/Row). Annars kan enumeratorn misslyckas med att traversera alla celler korrekt (vissa element kan traverseras flera gånger eller hoppas över).

**Returns:**
java.util.Iterator - Cellernas enumerator
### merge() {#merge--}
```
public void merge()
```


Kombinerar ett område av celler till en enda cell.

**Remarks**

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i intervallet.

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Sätter ett värde i området, om lämpligt kommer värdet att konverteras till en annan datatyp och cellens talformat återställas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | java.lang.String | Indatavärde |
| isConverted | boolean | True: konverterad till annan datatyp om lämpligt. |
| setStyle | boolean | True: sätt talformatet till cellens stil när du konverterar till annan datatyp |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på området.

**Remarks**

Namngivet område stöds. Till exempel,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Ställer in konturkantlinjer runt ett område av celler med samma kantstil och färg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Borderstilen. |
| borderColor | [Color](../../com.aspose.cells/color) | Borderfärg. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Ställer in konturkantlinjer runt ett område av celler.

**Remarks**

Både längden på borderStyles och borderStyles måste vara 4. Ordningen på borderStyles och borderStyles måste vara top,bottom,left,right

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Borderstilar. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Borderfärger. |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Ställer in stilen för området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Style-objektet. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Ställer in värdena i intervallet.

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
### unMerge() {#unMerge--}
```
public void unMerge()
```


Ta bort sammanslagning av sammanslagna celler i detta område.

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


Förena intervallen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Intervallen. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


Förena ett annat intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | Intervallet. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


Förena ett annat intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intervall | java.lang.String | Intervallet. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

