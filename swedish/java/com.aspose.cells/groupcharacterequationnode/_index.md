---
title: "GroupCharacterEquationNode"
second_title: "Aspose.Cells för Java API-referens"
description: "Denna klass specificerar Group-Character-funktionen som består av ett tecken placerat ovanför eller under text, ofta i syfte att visuellt gruppera objekt."
type: docs
url: /sv/java/com.aspose.cells/groupcharacterequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class GroupCharacterEquationNode extends EquationNode
```

Denna klass specificerar Group-Character-funktionen, bestående av ett tecken som ritas ovanför eller under text, ofta i syfte att visuellt gruppera objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. |
| [addChild(int equationType)](#addChild-int-) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Skapa en nod av den angivna typen. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
| [getChild(int index)](#getChild-int-) | Returnerar noden på det angivna indexet bland barnen till den aktuella noden. |
| [getChrType()](#getChrType--) | Specificera kombinerande tecken med typvärde. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Hämta ekvationstypen för den aktuella noden |
| [getFont()](#getFont--) | Returnerar teckensnittet för detta objekt. |
| [getGroupChr()](#getGroupChr--) | Specificerar en symbol (standard U+23DF). |
| [getLength()](#getLength--) | Hämtar längden på tecknen. |
| [getParentNode()](#getParentNode--) | Specificerar föräldranoden för den aktuella noden |
| [getPosition()](#getPosition--) | Detta attribut specificerar tecknets position i objektet |
| [getStartIndex()](#getStartIndex--) | Hämtar startindexet för tecknen. |
| [getTextOptions()](#getTextOptions--) | Returnerar textalternativen. |
| [getType()](#getType--) | Representerar nodens typ. |
| [getVertJc()](#getVertJc--) | Detta attribut, kombinerat med pos för groupChrPr, specificerar den vertikala layouten för groupChr-objektet. |
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
| [setChrType(int value)](#setChrType-int-) | Specificera kombinerande tecken med typvärde. |
| [setGroupChr(String value)](#setGroupChr-java.lang.String-) | Specificerar en symbol (standard U+23DF). |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Specificerar föräldranoden för den aktuella noden |
| [setPosition(int value)](#setPosition-int-) | Detta attribut specificerar tecknets position i objektet |
| [setVertJc(int value)](#setVertJc-int-) | Detta attribut, kombinerat med pos för groupChrPr, specificerar den vertikala layouten för groupChr-objektet. |
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
### getChrType() {#getChrType--}
```
public int getChrType()
```


Specificera kombinerande tecken med typvärde.

Se [EquationCombiningCharacterType](../../com.aspose.cells/equationcombiningcharactertype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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
### getGroupChr() {#getGroupChr--}
```
public String getGroupChr()
```


Specificerar en symbol (standard U+23DF). Det rekommenderas starkt att använda attributet ChrType för att ange accenttecken. Använd denna egenskap om du inte kan hitta det tecken du behöver i en känd typ.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Returns:**
java.lang.String
### getLength() {#getLength--}
```
public int getLength()
```


Hämtar längden på tecknen.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Specificerar föräldranoden för den aktuella noden

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Detta attribut specificerar tecknets position i objektet

Se [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Returns:**
int
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
### getVertJc() {#getVertJc--}
```
public int getVertJc()
```


Detta attribut, kombinerat med pos för groupChrPr, specificerar den vertikala layouten för groupChr-objektet. Där pos anger positionen för grupperingstecknet, anger vertJc justeringen av objektet i förhållande till baslinjen.

Se [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

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

### setChrType(int value) {#setChrType-int-}
```
public void setChrType(int value)
```


Specificera kombinerande tecken med typvärde.

Se [EquationCombiningCharacterType](../../com.aspose.cells/equationcombiningcharactertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setGroupChr(String value) {#setGroupChr-java.lang.String-}
```
public void setGroupChr(String value)
```


Specificerar en symbol (standard U+23DF). Det rekommenderas starkt att använda attributet ChrType för att ange accenttecken. Använd denna egenskap om du inte kan hitta det tecken du behöver i en känd typ.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Specificerar föräldranoden för den aktuella noden

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Detta attribut specificerar tecknets position i objektet

Se [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVertJc(int value) {#setVertJc-int-}
```
public void setVertJc(int value)
```


Detta attribut, kombinerat med pos för groupChrPr, specificerar den vertikala layouten för groupChr-objektet. Där pos anger positionen för grupperingstecknet, anger vertJc justeringen av objektet i förhållande till baslinjen.

Se [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

