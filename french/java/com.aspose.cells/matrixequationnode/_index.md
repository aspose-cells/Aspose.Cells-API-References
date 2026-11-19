---
title: "MatrixEquationNode"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Cette classe spécifie l'équation Matrix composée d'un ou plusieurs éléments disposés sur une ou plusieurs lignes et une ou plusieurs colonnes."
type: docs
url: /fr/java/com.aspose.cells/matrixequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class MatrixEquationNode extends EquationNode
```

Cette classe spécifie l'équation de matrice, composée d'un ou plusieurs éléments disposés sur une ou plusieurs lignes et une ou plusieurs colonnes.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Insère le nœud spécifié à la fin de la liste des nœuds enfants du nœud actuel. |
| [addChild(int equationType)](#addChild-int-) | Insère un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Crée un nœud du type spécifié. |
| [equals(Object obj)](#equals-java.lang.Object-) | Détermine si le nœud d'équation actuel est égal au nœud spécifié |
| [getBaseJc()](#getBaseJc--) | Cet attribut spécifie l'alignement de la matrice. |
| [getChild(int index)](#getChild-int-) | Renvoie le nœud à l'index spécifié parmi les enfants du nœud actuel. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Obtenez le type d'équation du nœud actuel |
| [getFont()](#getFont--) | Renvoie la police de cet objet. |
| [getLength()](#getLength--) | Obtient la longueur des caractères. |
| [getParentNode()](#getParentNode--) | Spécifie le nœud parent du nœud actuel |
| [getStartIndex()](#getStartIndex--) | Obtient l'index de départ des caractères. |
| [getTextOptions()](#getTextOptions--) | Renvoie les options de texte. |
| [getType()](#getType--) | Représente le type du nœud. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Insère le nœud spécifié après le nœud actuel. |
| [insertBefore(int equationType)](#insertBefore-int-) | Insère le nœud spécifié avant le nœud actuel. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Insère un nœud du type spécifié à la position d'index spécifiée dans la liste des nœuds enfants du nœud actuel. |
| [isHidePlaceholder()](#isHidePlaceholder--) | Cet attribut spécifie la propriété Hide Placeholders sur une matrice. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Se supprime du parent. |
| [removeAllChildren()](#removeAllChildren--) | Supprime tous les nœuds enfants du nœud actuel. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Supprime le nœud spécifié des enfants du nœud actuel. |
| [removeChild(int index)](#removeChild-int-) | Supprime le nœud à l'index spécifié des enfants du nœud actuel. |
| [setBaseJc(int value)](#setBaseJc-int-) | Cet attribut spécifie l'alignement de la matrice. |
| [setHidePlaceholder(boolean value)](#setHidePlaceholder-boolean-) | Cet attribut spécifie la propriété Hide Placeholders sur une matrice. |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Spécifie le nœud parent du nœud actuel |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Définit le style WordArt prédéfini. |
| [toLaTeX()](#toLaTeX--) | Convertissez cette equtation en expression LaTeX. |
| [toMathML()](#toMathML--) | Convertissez cette equtation en expression MathML. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


Insère le nœud spécifié à la fin de la liste des nœuds enfants du nœud actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Le nœud spécifié |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


Insère un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types de nœuds d'équation |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


Crée un nœud du type spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types de nœuds d'équation |
| workbook | [Workbook](../../com.aspose.cells/workbook) | L'objet classeur associé à l'équation |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | Le nœud parent où ce nœud est situé |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Détermine si le nœud d'équation actuel est égal au nœud spécifié

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | Le nœud spécifié |

**Returns:**
boolean -
### getBaseJc() {#getBaseJc--}
```
public int getBaseJc()
```


Cet attribut spécifie l'alignement de la matrice. Le texte en dehors de la matrice peut être aligné avec le bas, le haut ou le centre d'une fonction de matrice. Par défaut, la matrice utilise l'alignement centré.

Voir [EquationVerticalJustificationType](../../com.aspose.cells/equationverticaljustificationtype).

**Returns:**
int
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


Renvoie le nœud à l'index spécifié parmi les enfants du nœud actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Index du nœud |

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


Obtenez le type d'équation du nœud actuel

Voir [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Renvoie la police de cet objet.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Obtient la longueur des caractères.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Spécifie le nœud parent du nœud actuel

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Obtient l'index de départ des caractères.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Renvoie les options de texte.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Représente le type du nœud.

Voir [TextNodeType](../../com.aspose.cells/textnodetype).

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


Insère le nœud spécifié après le nœud actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types de nœuds d'équation |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


Insère le nœud spécifié avant le nœud actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types de nœuds d'équation |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


Insère un nœud du type spécifié à la position d'index spécifiée dans la liste des nœuds enfants du nœud actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | valeur d'index |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Types de nœuds d'équation |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### isHidePlaceholder() {#isHidePlaceholder--}
```
public boolean isHidePlaceholder()
```


Cet attribut spécifie la propriété Hide Placeholders sur une matrice. Lorsque cette propriété est activée, les espaces réservés n'apparaissent pas dans la matrice. Par défaut, les espaces réservés apparaissent de sorte que les emplacements où le texte peut être inséré soient visibles.

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


Se supprime du parent.

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


Supprime tous les nœuds enfants du nœud actuel.

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


Supprime le nœud spécifié des enfants du nœud actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Nœud à supprimer. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


Supprime le nœud à l'index spécifié des enfants du nœud actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Index du nœud |

### setBaseJc(int value) {#setBaseJc-int-}
```
public void setBaseJc(int value)
```


Cet attribut spécifie l'alignement de la matrice. Le texte en dehors de la matrice peut être aligné avec le bas, le haut ou le centre d'une fonction de matrice. Par défaut, la matrice utilise l'alignement centré.

Voir [EquationVerticalJustificationType](../../com.aspose.cells/equationverticaljustificationtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHidePlaceholder(boolean value) {#setHidePlaceholder-boolean-}
```
public void setHidePlaceholder(boolean value)
```


Cet attribut spécifie la propriété Hide Placeholders sur une matrice. Lorsque cette propriété est activée, les espaces réservés n'apparaissent pas dans la matrice. Par défaut, les espaces réservés apparaissent de sorte que les emplacements où le texte peut être inséré soient visibles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Spécifie le nœud parent du nœud actuel

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Définit le style WordArt prédéfini.

**Remarks**

Uniquement pour le texte de la forme/graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Le style WordArt prédéfini. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


Convertissez cette equtation en expression LaTeX.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


Convertissez cette equtation en expression MathML.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

