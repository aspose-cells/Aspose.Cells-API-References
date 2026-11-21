---
title: "DelimiterEquationNode"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Esta clase especifica la ecuación de delimitador que consiste en delimitadores de apertura y cierre, como paréntesis, llaves, corchetes y barras verticales, y un componente contenido dentro."
type: docs
url: /es/java/com.aspose.cells/delimiterequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class DelimiterEquationNode extends EquationNode
```

Esta clase especifica la ecuación de delimitador, que consiste en delimitadores de apertura y cierre (como paréntesis, llaves, corchetes y barras verticales), y un componente contenido dentro. El delimitador puede tener más de un componente, con un carácter separador designado entre cada componente.
## Métodos

| Método | Descripción |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Inserta el nodo especificado al final de la lista de nodos hijos del nodo actual. |
| [addChild(int equationType)](#addChild-int-) | Inserta un nodo del tipo especificado al final de la lista de nodos hijos del nodo actual. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Crea un nodo del tipo especificado. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina si el nodo de ecuación actual es igual al nodo especificado |
| [getBeginChar()](#getBeginChar--) | Carácter inicial del delimitador. |
| [getChild(int index)](#getChild-int-) | Devuelve el nodo en el índice especificado entre los hijos del nodo actual. |
| [getClass()](#getClass--) |  |
| [getDelimiterShape()](#getDelimiterShape--) | Especifica la forma de los delimitadores en el objeto delimitador. |
| [getEndChar()](#getEndChar--) | Carácter final del delimitador. |
| [getEquationType()](#getEquationType--) | Obtén el tipo de ecuación del nodo actual |
| [getFont()](#getFont--) | Devuelve la fuente de este objeto. |
| [getLength()](#getLength--) | Obtiene la longitud de los caracteres. |
| [getNaryGrow()](#getNaryGrow--) | Especifica si el delimitador debe expandirse y contraerse automáticamente con la altura de la fórmula. |
| [getParentNode()](#getParentNode--) | Especifica el nodo padre del nodo actual |
| [getSeparatorChar()](#getSeparatorChar--) | Carácter separador del delimitador. |
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
| [setBeginChar(String value)](#setBeginChar-java.lang.String-) | Carácter inicial del delimitador. |
| [setDelimiterShape(int value)](#setDelimiterShape-int-) | Especifica la forma de los delimitadores en el objeto delimitador. |
| [setEndChar(String value)](#setEndChar-java.lang.String-) | Carácter final del delimitador. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | Especifica si el delimitador debe expandirse y contraerse automáticamente con la altura de la fórmula. |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Especifica el nodo padre del nodo actual |
| [setSeparatorChar(String value)](#setSeparatorChar-java.lang.String-) | Carácter separador del delimitador. |
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
### getBeginChar() {#getBeginChar--}
```
public String getBeginChar()
```


Carácter inicial del delimitador.

**Remarks**

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

**Returns:**
java.lang.String
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
### getDelimiterShape() {#getDelimiterShape--}
```
public int getDelimiterShape()
```


Especifica la forma de los delimitadores en el objeto delimitador.

Ver [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).

**Returns:**
int
### getEndChar() {#getEndChar--}
```
public String getEndChar()
```


Carácter final del delimitador.

**Remarks**

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

**Returns:**
java.lang.String
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
### getLength() {#getLength--}
```
public int getLength()
```


Obtiene la longitud de los caracteres.

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


Especifica si el delimitador debe expandirse y contraerse automáticamente con la altura de la fórmula.

**Remarks**

Esta propiedad especifica la propiedad de crecimiento del delimitador a nivel de documento. Cuando está desactivada, el delimitador no crecerá para coincidir con el tamaño de la altura de su componente. Cuando está habilitada, el delimitador crece verticalmente para coincidir con la altura de su componente.

**Returns:**
boolean
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Especifica el nodo padre del nodo actual

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getSeparatorChar() {#getSeparatorChar--}
```
public String getSeparatorChar()
```


Carácter separador del delimitador.

**Remarks**

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

**Returns:**
java.lang.String
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

### setBeginChar(String value) {#setBeginChar-java.lang.String-}
```
public void setBeginChar(String value)
```


Carácter inicial del delimitador.

**Remarks**

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDelimiterShape(int value) {#setDelimiterShape-int-}
```
public void setDelimiterShape(int value)
```


Especifica la forma de los delimitadores en el objeto delimitador.

Ver [EquationDelimiterShapeType](../../com.aspose.cells/equationdelimitershapetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEndChar(String value) {#setEndChar-java.lang.String-}
```
public void setEndChar(String value)
```


Carácter final del delimitador.

**Remarks**

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


Especifica si el delimitador debe expandirse y contraerse automáticamente con la altura de la fórmula.

**Remarks**

Esta propiedad especifica la propiedad de crecimiento del delimitador a nivel de documento. Cuando está desactivada, el delimitador no crecerá para coincidir con el tamaño de la altura de su componente. Cuando está habilitada, el delimitador crece verticalmente para coincidir con la altura de su componente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Especifica el nodo padre del nodo actual

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setSeparatorChar(String value) {#setSeparatorChar-java.lang.String-}
```
public void setSeparatorChar(String value)
```


Carácter separador del delimitador.

**Remarks**

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

