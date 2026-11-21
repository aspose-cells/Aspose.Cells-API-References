---
title: "NaryEquationNode"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Esta clase especifica una ecuación de operador n-ario que consiste en un operador n-ario, una base u operando y límites superior e inferior opcionales."
type: docs
url: /es/java/com.aspose.cells/naryequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class NaryEquationNode extends EquationNode
```

Esta clase especifica una ecuación de operador n-ario que consta de un operador n-ario, una base (u operando) y límites superior e inferior opcionales.
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
| [getLength()](#getLength--) | Obtiene la longitud de los caracteres. |
| [getLimitLocation()](#getLimitLocation--) | Este atributo especifica la ubicación de los límites en operadores n-arios. |
| [getNaryGrow()](#getNaryGrow--) | Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. |
| [getNaryOperator()](#getNaryOperator--) | un operador n-ario.e.g "\u922d?. |
| [getNaryOperatorType()](#getNaryOperatorType--) | un operador n-ario.e.g "\u922d? |
| [getParentNode()](#getParentNode--) | Especifica el nodo padre del nodo actual |
| [getStartIndex()](#getStartIndex--) | Obtiene el índice de inicio de los caracteres. |
| [getTextOptions()](#getTextOptions--) | Devuelve las opciones de texto. |
| [getType()](#getType--) | Representa el tipo del nodo. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Inserta el nodo especificado después del nodo actual. |
| [insertBefore(int equationType)](#insertBefore-int-) | Inserta el nodo especificado antes del nodo actual. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Inserta un nodo del tipo especificado en la posición de índice especificada en la lista de nodos hijos del nodo actual. |
| [isHideSubscript()](#isHideSubscript--) | Mostrar el límite inferior |
| [isHideSuperscript()](#isHideSuperscript--) | Mostrar el límite superior |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Se elimina a sí mismo del padre. |
| [removeAllChildren()](#removeAllChildren--) | Elimina todos los nodos hijos del nodo actual. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Elimina el nodo especificado de los hijos del nodo actual. |
| [removeChild(int index)](#removeChild-int-) | Elimina el nodo en el índice especificado de los hijos del nodo actual. |
| [setHideSubscript(boolean value)](#setHideSubscript-boolean-) | Mostrar el límite inferior |
| [setHideSuperscript(boolean value)](#setHideSuperscript-boolean-) | Mostrar el límite superior |
| [setLimitLocation(int value)](#setLimitLocation-int-) | Este atributo especifica la ubicación de los límites en operadores n-arios. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. |
| [setNaryOperator(String value)](#setNaryOperator-java.lang.String-) | un operador n-ario.e.g "\u922d?. |
| [setNaryOperatorType(int value)](#setNaryOperatorType-int-) | un operador n-ario.e.g "\u922d? |
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
### getLength() {#getLength--}
```
public int getLength()
```


Obtiene la longitud de los caracteres.

**Returns:**
int
### getLimitLocation() {#getLimitLocation--}
```
public int getLimitLocation()
```


Este atributo especifica la ubicación de los límites en operadores n-arios. Los límites pueden estar centrados arriba y abajo del operador n-ario, o posicionados justo a la derecha del operador.

Ver [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. Cuando está desactivado, los operadores n-arios como integrales y sumas no crecen para coincidir con la altura de sus operandos. Cuando está activado, el operador n-ario crece verticalmente para coincidir con la altura de su operando.

**Returns:**
boolean
### getNaryOperator() {#getNaryOperator--}
```
public String getNaryOperator()
```


un operador n-ario, p.ej. "\\u922d?. Se recomienda encarecidamente usar el atributo NaryOperatorType para establecer el operador n-ario. Use esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido.

**Remarks**

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

**Returns:**
java.lang.String
### getNaryOperatorType() {#getNaryOperatorType--}
```
public int getNaryOperatorType()
```


un operador n-ario.e.g "\u922d?

Ver [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

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
### isHideSubscript() {#isHideSubscript--}
```
public boolean isHideSubscript()
```


Mostrar el límite inferior

**Returns:**
boolean
### isHideSuperscript() {#isHideSuperscript--}
```
public boolean isHideSuperscript()
```


Mostrar el límite superior

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

### setHideSubscript(boolean value) {#setHideSubscript-boolean-}
```
public void setHideSubscript(boolean value)
```


Mostrar el límite inferior

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHideSuperscript(boolean value) {#setHideSuperscript-boolean-}
```
public void setHideSuperscript(boolean value)
```


Mostrar el límite superior

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLimitLocation(int value) {#setLimitLocation-int-}
```
public void setLimitLocation(int value)
```


Este atributo especifica la ubicación de los límites en operadores n-arios. Los límites pueden estar centrados arriba y abajo del operador n-ario, o posicionados justo a la derecha del operador.

Ver [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


Este atributo especifica la propiedad de crecimiento de los operadores n-arios a nivel de documento. Cuando está desactivado, los operadores n-arios como integrales y sumas no crecen para coincidir con la altura de sus operandos. Cuando está activado, el operador n-ario crece verticalmente para coincidir con la altura de su operando.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNaryOperator(String value) {#setNaryOperator-java.lang.String-}
```
public void setNaryOperator(String value)
```


un operador n-ario, p.ej. "\\u922d?. Se recomienda encarecidamente usar el atributo NaryOperatorType para establecer el operador n-ario. Use esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido.

**Remarks**

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNaryOperatorType(int value) {#setNaryOperatorType-int-}
```
public void setNaryOperatorType(int value)
```


un operador n-ario.e.g "\u922d?

Ver [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

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

