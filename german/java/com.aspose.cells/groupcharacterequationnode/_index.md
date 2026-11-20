---
title: "GroupCharacterEquationNode"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Diese Klasse definiert die Group-Character-Funktion, die aus einem über oder unter dem Text platzierten Zeichen besteht, häufig mit dem Zweck, Elemente visuell zu gruppieren."
type: docs
url: /de/java/com.aspose.cells/groupcharacterequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class GroupCharacterEquationNode extends EquationNode
```

Diese Klasse spezifiziert die Group-Character-Funktion, die aus einem Zeichen besteht, das über oder unter dem Text gezeichnet wird, oft mit dem Zweck, Elemente visuell zu gruppieren.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Fügt den angegebenen Knoten am Ende der Kindknotenliste des aktuellen Knotens ein. |
| [addChild(int equationType)](#addChild-int-) | Fügt einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Erstelle einen Knoten des angegebenen Typs. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist |
| [getChild(int index)](#getChild-int-) | Gibt den Knoten am angegebenen Index unter den Kindknoten des aktuellen Knotens zurück. |
| [getChrType()](#getChrType--) | Geben Sie kombinierende Zeichen anhand des Typwerts an. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Erhalte den Gleichungstyp des aktuellen Knotens |
| [getFont()](#getFont--) | Gibt die Schriftart dieses Objekts zurück. |
| [getGroupChr()](#getGroupChr--) | Gibt ein Symbol an (Standard U+23DF). |
| [getLength()](#getLength--) | Ermittelt die Länge der Zeichen. |
| [getParentNode()](#getParentNode--) | Gibt den übergeordneten Knoten des aktuellen Knotens an |
| [getPosition()](#getPosition--) | Dieses Attribut gibt die Position des Zeichens im Objekt an. |
| [getStartIndex()](#getStartIndex--) | Ermittelt den Startindex der Zeichen. |
| [getTextOptions()](#getTextOptions--) | Gibt die Textoptionen zurück. |
| [getType()](#getType--) | Stellt den Typ des Knotens dar. |
| [getVertJc()](#getVertJc--) | Dieses Attribut, kombiniert mit pos von groupChrPr, gibt das vertikale Layout des groupChr-Objekts an. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Fügt den angegebenen Knoten nach dem aktuellen Knoten ein. |
| [insertBefore(int equationType)](#insertBefore-int-) | Fügt den angegebenen Knoten vor dem aktuellen Knoten ein. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Fügt einen Knoten des angegebenen Typs an der angegebenen Indexposition in die Kindknotenliste des aktuellen Knotens ein. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Entfernt sich selbst vom übergeordneten Element. |
| [removeAllChildren()](#removeAllChildren--) | Entfernt alle Kindknoten des aktuellen Knotens. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Entfernt den angegebenen Knoten aus den Kindknoten des aktuellen Knotens. |
| [removeChild(int index)](#removeChild-int-) | Entfernt den Knoten am angegebenen Index aus den Kindknoten des aktuellen Knotens. |
| [setChrType(int value)](#setChrType-int-) | Geben Sie kombinierende Zeichen anhand des Typwerts an. |
| [setGroupChr(String value)](#setGroupChr-java.lang.String-) | Gibt ein Symbol an (Standard U+23DF). |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Gibt den übergeordneten Knoten des aktuellen Knotens an |
| [setPosition(int value)](#setPosition-int-) | Dieses Attribut gibt die Position des Zeichens im Objekt an. |
| [setVertJc(int value)](#setVertJc-int-) | Dieses Attribut, kombiniert mit pos von groupChrPr, gibt das vertikale Layout des groupChr-Objekts an. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Legt den vordefinierten WordArt-Stil fest. |
| [toLaTeX()](#toLaTeX--) | Konvertieren Sie diese Gleichung in einen LaTeX-Ausdruck. |
| [toMathML()](#toMathML--) | Konvertieren Sie diese Gleichung in einen MathML-Ausdruck. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


Fügt den angegebenen Knoten am Ende der Kindknotenliste des aktuellen Knotens ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Der angegebene Knoten |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


Fügt einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typen von Gleichungsknoten |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


Erstelle einen Knoten des angegebenen Typs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typen von Gleichungsknoten |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Das Arbeitsmappenobjekt, das mit der Gleichung verknüpft ist |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | Der übergeordnete Knoten, in dem sich dieser Knoten befindet |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Der angegebene Knoten |

**Returns:**
boolean -
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


Gibt den Knoten am angegebenen Index unter den Kindknoten des aktuellen Knotens zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Index des Knotens |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - Returns the corresponding node if the specified node exists, otherwise returns null.
### getChrType() {#getChrType--}
```
public int getChrType()
```


Geben Sie kombinierende Zeichen anhand des Typwerts an.

Siehe [EquationCombiningCharacterType](../../com.aspose.cells/equationcombiningcharactertype).

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


Erhalte den Gleichungstyp des aktuellen Knotens

Siehe [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Gibt die Schriftart dieses Objekts zurück.

**Returns:**
[Font](../../com.aspose.cells/font)
### getGroupChr() {#getGroupChr--}
```
public String getGroupChr()
```


Gibt ein Symbol an (Standard U+23DF). Es wird dringend empfohlen, das Attribut ChrType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können.

**Remarks**

Es sollte beachtet werden, dass diese Eigenschaft nur ein Zeichen akzeptiert und bei mehreren übergebenen Zeichen nur das erste Zeichen akzeptiert wird.

**Returns:**
java.lang.String
### getLength() {#getLength--}
```
public int getLength()
```


Ermittelt die Länge der Zeichen.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Gibt den übergeordneten Knoten des aktuellen Knotens an

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Dieses Attribut gibt die Position des Zeichens im Objekt an.

Siehe [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Ermittelt den Startindex der Zeichen.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Gibt die Textoptionen zurück.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Stellt den Typ des Knotens dar.

Siehe [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### getVertJc() {#getVertJc--}
```
public int getVertJc()
```


Dieses Attribut, kombiniert mit pos von groupChrPr, gibt das vertikale Layout des groupChr-Objekts an. Dabei gibt pos die Position des Gruppierungszeichens an, vertJc gibt die Ausrichtung des Objekts relativ zur Grundlinie an.

Siehe [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

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


Fügt den angegebenen Knoten nach dem aktuellen Knoten ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typen von Gleichungsknoten |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


Fügt den angegebenen Knoten vor dem aktuellen Knoten ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typen von Gleichungsknoten |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


Fügt einen Knoten des angegebenen Typs an der angegebenen Indexposition in die Kindknotenliste des aktuellen Knotens ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Indexwert |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Typen von Gleichungsknoten |

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


Entfernt sich selbst vom übergeordneten Element.

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


Entfernt alle Kindknoten des aktuellen Knotens.

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


Entfernt den angegebenen Knoten aus den Kindknoten des aktuellen Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Zu löschender Knoten. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


Entfernt den Knoten am angegebenen Index aus den Kindknoten des aktuellen Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Index des Knotens |

### setChrType(int value) {#setChrType-int-}
```
public void setChrType(int value)
```


Geben Sie kombinierende Zeichen anhand des Typwerts an.

Siehe [EquationCombiningCharacterType](../../com.aspose.cells/equationcombiningcharactertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setGroupChr(String value) {#setGroupChr-java.lang.String-}
```
public void setGroupChr(String value)
```


Gibt ein Symbol an (Standard U+23DF). Es wird dringend empfohlen, das Attribut ChrType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können.

**Remarks**

Es sollte beachtet werden, dass diese Eigenschaft nur ein Zeichen akzeptiert und bei mehreren übergebenen Zeichen nur das erste Zeichen akzeptiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Gibt den übergeordneten Knoten des aktuellen Knotens an

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Dieses Attribut gibt die Position des Zeichens im Objekt an.

Siehe [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVertJc(int value) {#setVertJc-int-}
```
public void setVertJc(int value)
```


Dieses Attribut, kombiniert mit pos von groupChrPr, gibt das vertikale Layout des groupChr-Objekts an. Dabei gibt pos die Position des Gruppierungszeichens an, vertJc gibt die Ausrichtung des Objekts relativ zur Grundlinie an.

Siehe [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Legt den vordefinierten WordArt-Stil fest.

**Remarks**

Nur für den Text von Form/Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Der voreingestellte WordArt-Stil. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


Konvertieren Sie diese Gleichung in einen LaTeX-Ausdruck.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


Konvertieren Sie diese Gleichung in einen MathML-Ausdruck.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

