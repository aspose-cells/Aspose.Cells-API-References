---
title: "NaryEquationNode"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Diese Klasse spezifiziert eine n-äre Operator-Gleichung, die aus einem n-ären Operator, einer Basis oder einem Operanden und optionalen oberen und unteren Grenzen besteht."
type: docs
url: /de/java/com.aspose.cells/naryequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class NaryEquationNode extends EquationNode
```

Diese Klasse spezifiziert eine n-äre Operatorgleichung, die aus einem n-ären Operator, einer Basis (oder Operand) und optionalen oberen und unteren Grenzen besteht.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Fügt den angegebenen Knoten am Ende der Kindknotenliste des aktuellen Knotens ein. |
| [addChild(int equationType)](#addChild-int-) | Fügt einen Knoten des angegebenen Typs am Ende der Kindknotenliste des aktuellen Knotens ein. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Erstelle einen Knoten des angegebenen Typs. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist |
| [getChild(int index)](#getChild-int-) | Gibt den Knoten am angegebenen Index unter den Kindknoten des aktuellen Knotens zurück. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Erhalte den Gleichungstyp des aktuellen Knotens |
| [getFont()](#getFont--) | Gibt die Schriftart dieses Objekts zurück. |
| [getLength()](#getLength--) | Ermittelt die Länge der Zeichen. |
| [getLimitLocation()](#getLimitLocation--) | Dieses Attribut gibt den Ort der Grenzen in n-ären Operatoren an. |
| [getNaryGrow()](#getNaryGrow--) | Dieses Attribut gibt die Wachstumseigenschaft von n-ären Operatoren auf Dokumentebene an. |
| [getNaryOperator()](#getNaryOperator--) | ein n-ärer Operator, z.B. \"\\u922d?. |
| [getNaryOperatorType()](#getNaryOperatorType--) | ein n-ärer Operator, z.B. \"\\u922d?. |
| [getParentNode()](#getParentNode--) | Gibt den übergeordneten Knoten des aktuellen Knotens an |
| [getStartIndex()](#getStartIndex--) | Ermittelt den Startindex der Zeichen. |
| [getTextOptions()](#getTextOptions--) | Gibt die Textoptionen zurück. |
| [getType()](#getType--) | Stellt den Typ des Knotens dar. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Fügt den angegebenen Knoten nach dem aktuellen Knoten ein. |
| [insertBefore(int equationType)](#insertBefore-int-) | Fügt den angegebenen Knoten vor dem aktuellen Knoten ein. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Fügt einen Knoten des angegebenen Typs an der angegebenen Indexposition in die Kindknotenliste des aktuellen Knotens ein. |
| [isHideSubscript()](#isHideSubscript--) | Ob die untere Grenze angezeigt werden soll |
| [isHideSuperscript()](#isHideSuperscript--) | Ob die obere Grenze angezeigt werden soll |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Entfernt sich selbst vom übergeordneten Element. |
| [removeAllChildren()](#removeAllChildren--) | Entfernt alle Kindknoten des aktuellen Knotens. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Entfernt den angegebenen Knoten aus den Kindknoten des aktuellen Knotens. |
| [removeChild(int index)](#removeChild-int-) | Entfernt den Knoten am angegebenen Index aus den Kindknoten des aktuellen Knotens. |
| [setHideSubscript(boolean value)](#setHideSubscript-boolean-) | Ob die untere Grenze angezeigt werden soll |
| [setHideSuperscript(boolean value)](#setHideSuperscript-boolean-) | Ob die obere Grenze angezeigt werden soll |
| [setLimitLocation(int value)](#setLimitLocation-int-) | Dieses Attribut gibt den Ort der Grenzen in n-ären Operatoren an. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | Dieses Attribut gibt die Wachstumseigenschaft von n-ären Operatoren auf Dokumentebene an. |
| [setNaryOperator(String value)](#setNaryOperator-java.lang.String-) | ein n-ärer Operator, z.B. \"\\u922d?. |
| [setNaryOperatorType(int value)](#setNaryOperatorType-int-) | ein n-ärer Operator, z.B. \"\\u922d?. |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Gibt den übergeordneten Knoten des aktuellen Knotens an |
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
### getLength() {#getLength--}
```
public int getLength()
```


Ermittelt die Länge der Zeichen.

**Returns:**
int
### getLimitLocation() {#getLimitLocation--}
```
public int getLimitLocation()
```


Dieses Attribut gibt den Ort der Grenzen in n-ären Operatoren an. Grenzen können entweder zentriert über und unter dem n-ären Operator liegen oder direkt rechts vom Operator positioniert werden.

Siehe [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


Dieses Attribut gibt die Wachstumseigenschaft von n-ären Operatoren auf Dokumentebene an. Wenn deaktiviert, wachsen n-äre Operatoren wie Integrale und Summen nicht, um die Höhe ihres Operanden anzupassen. Wenn aktiviert, wächst der n-äre Operator vertikal, um die Höhe seines Operanden anzupassen.

**Returns:**
boolean
### getNaryOperator() {#getNaryOperator--}
```
public String getNaryOperator()
```


ein n-ärer Operator, z.B. \"\\u922d?. Es wird dringend empfohlen, das Attribut **NaryOperatorType** zu verwenden, um den n-ären Operator festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können.

**Remarks**

Es sollte beachtet werden, dass diese Eigenschaft nur ein Zeichen akzeptiert und bei mehreren übergebenen Zeichen nur das erste Zeichen akzeptiert wird.

**Returns:**
java.lang.String
### getNaryOperatorType() {#getNaryOperatorType--}
```
public int getNaryOperatorType()
```


ein n-ärer Operator, z.B. \"\\u922d?.

Siehe [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Gibt den übergeordneten Knoten des aktuellen Knotens an

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
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
### isHideSubscript() {#isHideSubscript--}
```
public boolean isHideSubscript()
```


Ob die untere Grenze angezeigt werden soll

**Returns:**
boolean
### isHideSuperscript() {#isHideSuperscript--}
```
public boolean isHideSuperscript()
```


Ob die obere Grenze angezeigt werden soll

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

### setHideSubscript(boolean value) {#setHideSubscript-boolean-}
```
public void setHideSubscript(boolean value)
```


Ob die untere Grenze angezeigt werden soll

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHideSuperscript(boolean value) {#setHideSuperscript-boolean-}
```
public void setHideSuperscript(boolean value)
```


Ob die obere Grenze angezeigt werden soll

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLimitLocation(int value) {#setLimitLocation-int-}
```
public void setLimitLocation(int value)
```


Dieses Attribut gibt den Ort der Grenzen in n-ären Operatoren an. Grenzen können entweder zentriert über und unter dem n-ären Operator liegen oder direkt rechts vom Operator positioniert werden.

Siehe [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


Dieses Attribut gibt die Wachstumseigenschaft von n-ären Operatoren auf Dokumentebene an. Wenn deaktiviert, wachsen n-äre Operatoren wie Integrale und Summen nicht, um die Höhe ihres Operanden anzupassen. Wenn aktiviert, wächst der n-äre Operator vertikal, um die Höhe seines Operanden anzupassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNaryOperator(String value) {#setNaryOperator-java.lang.String-}
```
public void setNaryOperator(String value)
```


ein n-ärer Operator, z.B. \"\\u922d?. Es wird dringend empfohlen, das Attribut **NaryOperatorType** zu verwenden, um den n-ären Operator festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können.

**Remarks**

Es sollte beachtet werden, dass diese Eigenschaft nur ein Zeichen akzeptiert und bei mehreren übergebenen Zeichen nur das erste Zeichen akzeptiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNaryOperatorType(int value) {#setNaryOperatorType-int-}
```
public void setNaryOperatorType(int value)
```


ein n-ärer Operator, z.B. \"\\u922d?.

Siehe [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Gibt den übergeordneten Knoten des aktuellen Knotens an

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

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

