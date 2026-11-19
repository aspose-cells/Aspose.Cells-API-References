---
title: "GroupCharacterEquationNode"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Cette classe spécifie la fonction Group-Character consistant en un caractère dessiné au-dessus ou au-dessous du texte, souvent dans le but de regrouper visuellement les éléments."
type: docs
url: /fr/java/com.aspose.cells/groupcharacterequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class GroupCharacterEquationNode extends EquationNode
```

Cette classe spécifie la fonction Groupe-Caractère, consistant en un caractère dessiné au-dessus ou au-dessous du texte, souvent dans le but de regrouper visuellement les éléments.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Insère le nœud spécifié à la fin de la liste des nœuds enfants du nœud actuel. |
| [addChild(int equationType)](#addChild-int-) | Insère un nœud du type spécifié à la fin de la liste des nœuds enfants du nœud actuel. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Crée un nœud du type spécifié. |
| [equals(Object obj)](#equals-java.lang.Object-) | Détermine si le nœud d'équation actuel est égal au nœud spécifié |
| [getChild(int index)](#getChild-int-) | Renvoie le nœud à l'index spécifié parmi les enfants du nœud actuel. |
| [getChrType()](#getChrType--) | Spécifiez les caractères combinés par valeur de type. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Obtenez le type d'équation du nœud actuel |
| [getFont()](#getFont--) | Renvoie la police de cet objet. |
| [getGroupChr()](#getGroupChr--) | Spécifie un symbole (par défaut U+23DF). |
| [getLength()](#getLength--) | Obtient la longueur des caractères. |
| [getParentNode()](#getParentNode--) | Spécifie le nœud parent du nœud actuel |
| [getPosition()](#getPosition--) | Cet attribut spécifie la position du caractère dans l'objet |
| [getStartIndex()](#getStartIndex--) | Obtient l'index de départ des caractères. |
| [getTextOptions()](#getTextOptions--) | Renvoie les options de texte. |
| [getType()](#getType--) | Représente le type du nœud. |
| [getVertJc()](#getVertJc--) | Cet attribut, combiné avec pos de groupChrPr, spécifie la disposition verticale de l'objet groupChr. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Insère le nœud spécifié après le nœud actuel. |
| [insertBefore(int equationType)](#insertBefore-int-) | Insère le nœud spécifié avant le nœud actuel. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Insère un nœud du type spécifié à la position d'index spécifiée dans la liste des nœuds enfants du nœud actuel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Se supprime du parent. |
| [removeAllChildren()](#removeAllChildren--) | Supprime tous les nœuds enfants du nœud actuel. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Supprime le nœud spécifié des enfants du nœud actuel. |
| [removeChild(int index)](#removeChild-int-) | Supprime le nœud à l'index spécifié des enfants du nœud actuel. |
| [setChrType(int value)](#setChrType-int-) | Spécifiez les caractères combinés par valeur de type. |
| [setGroupChr(String value)](#setGroupChr-java.lang.String-) | Spécifie un symbole (par défaut U+23DF). |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Spécifie le nœud parent du nœud actuel |
| [setPosition(int value)](#setPosition-int-) | Cet attribut spécifie la position du caractère dans l'objet |
| [setVertJc(int value)](#setVertJc-int-) | Cet attribut, combiné avec pos de groupChrPr, spécifie la disposition verticale de l'objet groupChr. |
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
### getChrType() {#getChrType--}
```
public int getChrType()
```


Spécifiez les caractères combinés par valeur de type.

Voir [EquationCombiningCharacterType](../../com.aspose.cells/equationcombiningcharactertype).

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
### getGroupChr() {#getGroupChr--}
```
public String getGroupChr()
```


Spécifie un symbole (par défaut U+23DF). Il est fortement recommandé d'utiliser l'attribut ChrType pour définir le caractère d'accent. Utilisez ce réglage de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu.

**Remarks**

Il convient de noter que cette propriété n'accepte qu'un seul caractère, et si plusieurs caractères sont fournis, seul le premier caractère est accepté.

**Returns:**
java.lang.String
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
### getPosition() {#getPosition--}
```
public int getPosition()
```


Cet attribut spécifie la position du caractère dans l'objet

Voir [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Returns:**
int
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
### getVertJc() {#getVertJc--}
```
public int getVertJc()
```


Cet attribut, combiné avec pos de groupChrPr, spécifie la disposition verticale de l'objet groupChr. Où pos indique la position du caractère de groupement, vertJc indique l'alignement de l'objet par rapport à la ligne de base.

Voir [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

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

### setChrType(int value) {#setChrType-int-}
```
public void setChrType(int value)
```


Spécifiez les caractères combinés par valeur de type.

Voir [EquationCombiningCharacterType](../../com.aspose.cells/equationcombiningcharactertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setGroupChr(String value) {#setGroupChr-java.lang.String-}
```
public void setGroupChr(String value)
```


Spécifie un symbole (par défaut U+23DF). Il est fortement recommandé d'utiliser l'attribut ChrType pour définir le caractère d'accent. Utilisez ce réglage de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu.

**Remarks**

Il convient de noter que cette propriété n'accepte qu'un seul caractère, et si plusieurs caractères sont fournis, seul le premier caractère est accepté.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Spécifie le nœud parent du nœud actuel

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Cet attribut spécifie la position du caractère dans l'objet

Voir [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVertJc(int value) {#setVertJc-int-}
```
public void setVertJc(int value)
```


Cet attribut, combiné avec pos de groupChrPr, spécifie la disposition verticale de l'objet groupChr. Où pos indique la position du caractère de groupement, vertJc indique l'alignement de l'objet par rapport à la ligne de base.

Voir [EquationCharacterPositionType](../../com.aspose.cells/equationcharacterpositiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

