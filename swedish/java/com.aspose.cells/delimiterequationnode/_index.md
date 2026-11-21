---
title: "DelimiterEquationNode"
second_title: "Aspose.Cells för Java API-referens"
description: "Denna klass specificerar delimiterekvationen som består av öppnings- och stängningsavgränsare såsom parenteser, klammerparenteser, hakparenteser och vertikala streck samt en komponent som finns inuti."
type: docs
url: /sv/java/com.aspose.cells/delimiterequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class DelimiterEquationNode extends EquationNode
```

Denna klass specificerar delimiterekvationen, bestående av öppnings- och stängningsavgränsare (såsom parenteser, klammerparenteser, hakparenteser och vertikala streck) och en komponent som finns inuti. Avgränsaren kan ha mer än en komponent, med ett bestämt separator‑tecken mellan varje komponent.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. |
| [addChild(int equationType)](#addChild-int-) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Skapa en nod av den angivna typen. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
| [getBeginChar()](#getBeginChar--) | Inledande delimiter‑tecken. |
| [getChild(int index)](#getChild-int-) | Returnerar noden på det angivna indexet bland barnen till den aktuella noden. |
| [getClass()](#getClass--) |  |
| [getDelimiterShape()](#getDelimiterShape--) | Anger formen på avgränsare i avgränsningsobjektet. |
| [getEndChar()](#getEndChar--) | Avgränsningens avslutande tecken. |
| [getEquationType()](#getEquationType--) | Hämta ekvationstypen för den aktuella noden |
| [getFont()](#getFont--) | Returnerar teckensnittet för detta objekt. |
| [getLength()](#getLength--) | Hämtar längden på tecknen. |
| [getNaryGrow()](#getNaryGrow--) | Anger om avgränsaren automatiskt ska expandera och krympa i takt med formelns höjd. |
| [getParentNode()](#getParentNode--) | Specificerar föräldranoden för den aktuella noden |
| [getSeparatorChar()](#getSeparatorChar--) | Avgränsningens separator-tecken. |
| [getStartIndex()](#getStartIndex--) | Hämtar startindexet för tecknen. |
| [getTextOptions()](#getTextOptions--) | Returnerar textalternativen. |
| [getType()](#getType--) | Representerar nodens typ. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Infogar den angivna noden efter den aktuella noden. |
| [insertBefore(int equationType)](#insertBefore-int-) | Infogar den angivna noden före den aktuella noden. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens barnnodlista. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Tar bort sig själv från föräldern. |
| [removeAllChildren()](#removeAllChildren--) | Tar bort alla barnnoder för den aktuella noden. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Tar bort den angivna noden från den aktuella nodens barn. |
| [removeChild(int index)](#removeChild-int-) | Tar bort noden på det angivna indexet från den aktuella nodens barn. |
| [setBeginChar(String value)](#setBeginChar-java.lang.String-) | Inledande delimiter‑tecken. |
| [setDelimiterShape(int value)](#setDelimiterShape-int-) | Anger formen på avgränsare i avgränsningsobjektet. |
| [setEndChar(String value)](#setEndChar-java.lang.String-) | Avgränsningens avslutande tecken. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | Anger om avgränsaren automatiskt ska expandera och krympa i takt med formelns höjd. |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Specificerar föräldranoden för den aktuella noden |
| [setSeparatorChar(String value)](#setSeparatorChar-java.lang.String-) | Avgränsningens separator-tecken. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Ställer in den förinställda WordArt-stilen. |
| [toLaTeX()](#toLaTeX--) | Konvertera denna ekvation till ett LaTeX-uttryck. |
| [toMathML()](#toMathML--) | Konvertera denna ekvation till ett MathML-uttryck. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Den angivna noden |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typer av ekvationsnoder |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


Skapa en nod av den angivna typen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typer av ekvationsnoder |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Arbetsbokobjektet som är associerat med ekvationen |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | Föräldranoden där denna nod är placerad |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestäm om den aktuella ekvationsnoden är lika med den angivna noden

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Den angivna noden |

**Returns:**
boolean -
### getBeginChar() {#getBeginChar--}
```
public String getBeginChar()
```


Inledande delimiter‑tecken.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Returns:**
java.lang.String
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


Returnerar noden på det angivna indexet bland barnen till den aktuella noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Nodens index |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - Returns the corresponding node if the specified node exists, otherwise returns null.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDelimiterShape() {#getDelimiterShape--}
```
public int getDelimiterShape()
```


Anger formen på avgränsare i avgränsningsobjektet.

Se [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).

**Returns:**
int
### getEndChar() {#getEndChar--}
```
public String getEndChar()
```


Avgränsningens avslutande tecken.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Returns:**
java.lang.String
### getEquationType() {#getEquationType--}
```
public int getEquationType()
```


Hämta ekvationstypen för den aktuella noden

Se [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Returnerar teckensnittet för detta objekt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Hämtar längden på tecknen.

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


Anger om avgränsaren automatiskt ska expandera och krympa i takt med formelns höjd.

**Remarks**

Denna egenskap anger tillväxtegenskapen för avgränsaren på dokumentnivå. När den är avstängd kommer avgränsaren inte att växa för att matcha komponentens höjd. När den är aktiverad växer avgränsaren vertikalt för att matcha komponentens höjd.

**Returns:**
boolean
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Specificerar föräldranoden för den aktuella noden

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getSeparatorChar() {#getSeparatorChar--}
```
public String getSeparatorChar()
```


Avgränsningens separator-tecken.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Returns:**
java.lang.String
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Hämtar startindexet för tecknen.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Returnerar textalternativen.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Representerar nodens typ.

Se [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### insertAfter(int equationType) {#insertAfter-int-}
```
public EquationNode insertAfter(int equationType)
```


Infogar den angivna noden efter den aktuella noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typer av ekvationsnoder |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


Infogar den angivna noden före den aktuella noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typer av ekvationsnoder |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens barnnodlista.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexvärde |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typer av ekvationsnoder |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove() {#remove--}
```
public void remove()
```


Tar bort sig själv från föräldern.

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


Tar bort alla barnnoder för den aktuella noden.

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


Tar bort den angivna noden från den aktuella nodens barn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Nod som ska tas bort. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


Tar bort noden på det angivna indexet från den aktuella nodens barn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Nodens index |

### setBeginChar(String value) {#setBeginChar-java.lang.String-}
```
public void setBeginChar(String value)
```


Inledande delimiter‑tecken.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDelimiterShape(int value) {#setDelimiterShape-int-}
```
public void setDelimiterShape(int value)
```


Anger formen på avgränsare i avgränsningsobjektet.

Se [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEndChar(String value) {#setEndChar-java.lang.String-}
```
public void setEndChar(String value)
```


Avgränsningens avslutande tecken.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


Anger om avgränsaren automatiskt ska expandera och krympa i takt med formelns höjd.

**Remarks**

Denna egenskap anger tillväxtegenskapen för avgränsaren på dokumentnivå. När den är avstängd kommer avgränsaren inte att växa för att matcha komponentens höjd. När den är aktiverad växer avgränsaren vertikalt för att matcha komponentens höjd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Specificerar föräldranoden för den aktuella noden

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setSeparatorChar(String value) {#setSeparatorChar-java.lang.String-}
```
public void setSeparatorChar(String value)
```


Avgränsningens separator-tecken.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Ställer in den förinställda WordArt-stilen.

**Remarks**

Endast för texten i form/diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Den förinställda WordArt-stilen. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


Konvertera denna ekvation till ett LaTeX-uttryck.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


Konvertera denna ekvation till ett MathML-uttryck.

**Returns:**
java.lang.String -
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

