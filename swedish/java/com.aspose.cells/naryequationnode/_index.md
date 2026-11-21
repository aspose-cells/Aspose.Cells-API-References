---
title: "NaryEquationNode"
second_title: "Aspose.Cells för Java API-referens"
description: "Denna klass specificerar en n-ary operatorlikning som består av en n-ary operator, en bas eller operand och valfria övre och nedre gränser."
type: docs
url: /sv/java/com.aspose.cells/naryequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class NaryEquationNode extends EquationNode
```

Denna klass specificerar en n-är operatorlikning bestående av en n-är operator, en bas (eller operand) och valfria övre och nedre gränser.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. |
| [addChild(int equationType)](#addChild-int-) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Skapa en nod av den angivna typen. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
| [getChild(int index)](#getChild-int-) | Returnerar noden på det angivna indexet bland barnen till den aktuella noden. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Hämta ekvationstypen för den aktuella noden |
| [getFont()](#getFont--) | Returnerar teckensnittet för detta objekt. |
| [getLength()](#getLength--) | Hämtar längden på tecknen. |
| [getLimitLocation()](#getLimitLocation--) | Detta attribut specificerar placeringen av gränser i n-ary-operatorer. |
| [getNaryGrow()](#getNaryGrow--) | Detta attribut specificerar tillväxtsegenskapen för n-ary-operatorer på dokumentnivå. |
| [getNaryOperator()](#getNaryOperator--) | en n-ary operator.t.ex "\\u922d?. |
| [getNaryOperatorType()](#getNaryOperatorType--) | en n-är operator.t.ex "\u922d? |
| [getParentNode()](#getParentNode--) | Specificerar föräldranoden för den aktuella noden |
| [getStartIndex()](#getStartIndex--) | Hämtar startindexet för tecknen. |
| [getTextOptions()](#getTextOptions--) | Returnerar textalternativen. |
| [getType()](#getType--) | Representerar nodens typ. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Infogar den angivna noden efter den aktuella noden. |
| [insertBefore(int equationType)](#insertBefore-int-) | Infogar den angivna noden före den aktuella noden. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens barnnodlista. |
| [isHideSubscript()](#isHideSubscript--) | Om den nedre gränsen ska visas |
| [isHideSuperscript()](#isHideSuperscript--) | Om den övre gränsen ska visas |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Tar bort sig själv från föräldern. |
| [removeAllChildren()](#removeAllChildren--) | Tar bort alla barnnoder för den aktuella noden. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Tar bort den angivna noden från den aktuella nodens barn. |
| [removeChild(int index)](#removeChild-int-) | Tar bort noden på det angivna indexet från den aktuella nodens barn. |
| [setHideSubscript(boolean value)](#setHideSubscript-boolean-) | Om den nedre gränsen ska visas |
| [setHideSuperscript(boolean value)](#setHideSuperscript-boolean-) | Om den övre gränsen ska visas |
| [setLimitLocation(int value)](#setLimitLocation-int-) | Detta attribut specificerar placeringen av gränser i n-ary-operatorer. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | Detta attribut specificerar tillväxtsegenskapen för n-ary-operatorer på dokumentnivå. |
| [setNaryOperator(String value)](#setNaryOperator-java.lang.String-) | en n-ary operator.t.ex "\\u922d?. |
| [setNaryOperatorType(int value)](#setNaryOperatorType-int-) | en n-är operator.t.ex "\u922d? |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Specificerar föräldranoden för den aktuella noden |
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
### getLength() {#getLength--}
```
public int getLength()
```


Hämtar längden på tecknen.

**Returns:**
int
### getLimitLocation() {#getLimitLocation--}
```
public int getLimitLocation()
```


Detta attribut anger placeringen av gränser i n-är operatorer. Gränser kan antingen centreras ovanför och under n-är operatorn, eller placeras precis till höger om operatorn.

Se [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


Detta attribut anger tillväxtegenskapen för n-är operatorer på dokumentnivå. När den är avstängd växer inte n-är operatorer såsom integraler och summor för att matcha operandens höjd. När den är påslagen växer n-är operatorn vertikalt för att matcha operandens höjd.

**Returns:**
boolean
### getNaryOperator() {#getNaryOperator--}
```
public String getNaryOperator()
```


en n-är operator.t.ex "\u922d?. Det rekommenderas starkt att använda attributet NaryOperatorType för att ange n-är operator. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Returns:**
java.lang.String
### getNaryOperatorType() {#getNaryOperatorType--}
```
public int getNaryOperatorType()
```


en n-är operator.t.ex "\u922d?

Se [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Specificerar föräldranoden för den aktuella noden

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
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
### isHideSubscript() {#isHideSubscript--}
```
public boolean isHideSubscript()
```


Om den nedre gränsen ska visas

**Returns:**
boolean
### isHideSuperscript() {#isHideSuperscript--}
```
public boolean isHideSuperscript()
```


Om den övre gränsen ska visas

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

### setHideSubscript(boolean value) {#setHideSubscript-boolean-}
```
public void setHideSubscript(boolean value)
```


Om den nedre gränsen ska visas

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHideSuperscript(boolean value) {#setHideSuperscript-boolean-}
```
public void setHideSuperscript(boolean value)
```


Om den övre gränsen ska visas

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLimitLocation(int value) {#setLimitLocation-int-}
```
public void setLimitLocation(int value)
```


Detta attribut anger placeringen av gränser i n-är operatorer. Gränser kan antingen centreras ovanför och under n-är operatorn, eller placeras precis till höger om operatorn.

Se [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


Detta attribut anger tillväxtegenskapen för n-är operatorer på dokumentnivå. När den är avstängd växer inte n-är operatorer såsom integraler och summor för att matcha operandens höjd. När den är påslagen växer n-är operatorn vertikalt för att matcha operandens höjd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNaryOperator(String value) {#setNaryOperator-java.lang.String-}
```
public void setNaryOperator(String value)
```


en n-är operator.t.ex "\u922d?. Det rekommenderas starkt att använda attributet NaryOperatorType för att ange n-är operator. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ.

**Remarks**

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in accepteras endast det första tecknet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNaryOperatorType(int value) {#setNaryOperatorType-int-}
```
public void setNaryOperatorType(int value)
```


en n-är operator.t.ex "\u922d?

Se [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Specificerar föräldranoden för den aktuella noden

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

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

