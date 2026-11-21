---
title: "EquationNodeParagraph"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Esta clase especifica un párrafo matemático que contiene uno o más elementos MathEquationNodeOMath."
type: docs
url: /es/java/com.aspose.cells/equationnodeparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class EquationNodeParagraph extends EquationNode
```

Esta clase especifica un párrafo matemático que contiene uno o más elementos MathEquationNode(OMath).
## Métodos

| Método | Descripción |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual. |
| [addChild(int equationType)](#addChild-int-) | Inserta un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Crea un nodo del tipo especificado. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina si el nodo de ecuación actual es igual al nodo especificado |
| [getChild(int index)](#getChild-int-) | Devuelve el nodo en el índice especificado entre los hijos del nodo actual. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Obtén el tipo de ecuación del nodo actual |
| [getFont()](#getFont--) | Devuelve la fuente de este objeto. |
| [getJustification()](#getJustification--) | Esto especifica la justificación del párrafo matemático (una serie de ecuaciones adyacentes dentro del mismo párrafo). |
| [getLength()](#getLength--) | Obtiene la longitud de los caracteres. |
| [getParentNode()](#getParentNode--) | Especifica el nodo padre del nodo actual |
| [getStartIndex()](#getStartIndex--) | Obtiene el índice de inicio de los caracteres. |
| [getTextOptions()](#getTextOptions--) | Devuelve las opciones de texto. |
| [getType()](#getType--) | Representa el tipo del nodo. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Inserta el nodo especificado después del nodo actual. |
| [insertBefore(int equationType)](#insertBefore-int-) | Inserta el nodo especificado antes del nodo actual. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Inserta un nodo del tipo especificado en la posición de índice especificada en la lista de nodos hijos del nodo actual. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Se elimina a sí mismo del padre. |
| [removeAllChildren()](#removeAllChildren--) | Elimina todos los nodos hijos del nodo actual. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Elimina el nodo especificado de los hijos del nodo actual. |
| [removeChild(int index)](#removeChild-int-) | Elimina el nodo en el índice especificado de los hijos del nodo actual. |
| [setJustification(int value)](#setJustification-int-) | Esto especifica la justificación del párrafo matemático (una serie de ecuaciones adyacentes dentro del mismo párrafo). |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Especifica el nodo padre del nodo actual |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Establece el estilo WordArt predefinido. |
| [toLaTeX()](#toLaTeX--) | Convierte esta ecuación a una expresión LaTeX. |
| [toMathML()](#toMathML--) | Convierte esta ecuación a una expresión MathML. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | El nodo especificado |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


Inserta un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipos de nodos de ecuación |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


Crea un nodo del tipo especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipos de nodos de ecuación |
| workbook | [Workbook](../../com.aspose.cells/workbook) | El objeto de libro de trabajo asociado con la ecuación |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | El nodo padre donde se encuentra este nodo |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina si el nodo de ecuación actual es igual al nodo especificado

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El nodo especificado |

**Returns:**
boolean -
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


Devuelve el nodo en el índice especificado entre los hijos del nodo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | Índice del nodo |

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


Obtén el tipo de ecuación del nodo actual

Ver [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Devuelve la fuente de este objeto.

**Returns:**
[Font](../../com.aspose.cells/font)
### getJustification() {#getJustification--}
```
public int getJustification()
```


Esto especifica la justificación del párrafo matemático (una serie de ecuaciones adyacentes dentro del mismo párrafo). Un párrafo matemático puede estar Alineado a la Izquierda, Alineado a la Derecha, Centrado, o Centrado como Grupo. Por defecto, el párrafo matemático está Centrado como Grupo. Esto significa que las ecuaciones pueden alinearse entre sí, pero todo el grupo de ecuaciones está centrado como un todo.

Ver [EquationHorizontalJustificationType](../../com.aspose.cells/equationhorizontaljustificationtype).

**Returns:**
int
### getLength() {#getLength--}
```
public int getLength()
```


Obtiene la longitud de los caracteres.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Especifica el nodo padre del nodo actual

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Obtiene el índice de inicio de los caracteres.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Devuelve las opciones de texto.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Representa el tipo del nodo.

Ver [TextNodeType](../../com.aspose.cells/textnodetype).

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


Inserta el nodo especificado después del nodo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipos de nodos de ecuación |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


Inserta el nodo especificado antes del nodo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipos de nodos de ecuación |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


Inserta un nodo del tipo especificado en la posición de índice especificada en la lista de nodos hijos del nodo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | valor del índice |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Tipos de nodos de ecuación |

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


Se elimina a sí mismo del padre.

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


Elimina todos los nodos hijos del nodo actual.

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


Elimina el nodo especificado de los hijos del nodo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Nodo a eliminar. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


Elimina el nodo en el índice especificado de los hijos del nodo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | Índice del nodo |

### setJustification(int value) {#setJustification-int-}
```
public void setJustification(int value)
```


Esto especifica la justificación del párrafo matemático (una serie de ecuaciones adyacentes dentro del mismo párrafo). Un párrafo matemático puede estar Alineado a la Izquierda, Alineado a la Derecha, Centrado, o Centrado como Grupo. Por defecto, el párrafo matemático está Centrado como Grupo. Esto significa que las ecuaciones pueden alinearse entre sí, pero todo el grupo de ecuaciones está centrado como un todo.

Ver [EquationHorizontalJustificationType](../../com.aspose.cells/equationhorizontaljustificationtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Especifica el nodo padre del nodo actual

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Establece el estilo WordArt predefinido.

**Remarks**

Solo para el texto de forma/gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). El estilo WordArt predefinido. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


Convierte esta ecuación a una expresión LaTeX.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


Convierte esta ecuación a una expresión MathML.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

