---
title: "NaryEquationNode"
second_title: "Справочник API Aspose.Cells for Java"
description: "Этот класс определяет n-арный оператор уравнения, состоящий из n-арного оператора, базы или операнда, а также необязательных верхних и нижних границ."
type: docs
url: /ru/java/com.aspose.cells/naryequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class NaryEquationNode extends EquationNode
```

Этот класс задает уравнение n-арного оператора, состоящее из n-арного оператора, базы (или операнда) и необязательных верхних и нижних границ.
## Методы

| Метод | Описание |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Вставляет указанный узел в конец списка дочерних узлов текущего узла. |
| [addChild(int equationType)](#addChild-int-) | Вставьте узел указанного типа в конец списка дочерних узлов текущего узла. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Создайте узел указанного типа. |
| [equals(Object obj)](#equals-java.lang.Object-) | Определите, равен ли текущий узел уравнения указанному узлу |
| [getChild(int index)](#getChild-int-) | Возвращает узел с указанным индексом среди дочерних узлов текущего узла. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Получите тип уравнения текущего узла |
| [getFont()](#getFont--) | Возвращает шрифт этого объекта. |
| [getLength()](#getLength--) | Получает длину символов. |
| [getLimitLocation()](#getLimitLocation--) | Этот атрибут определяет расположение пределов в n-арных операторах. |
| [getNaryGrow()](#getNaryGrow--) | Этот атрибут определяет свойство роста n-арных операторов на уровне документа. |
| [getNaryOperator()](#getNaryOperator--) | n-арный оператор, например "\u922d?. |
| [getNaryOperatorType()](#getNaryOperatorType--) | n-арный оператор, например "\u922d? |
| [getParentNode()](#getParentNode--) | Указывает родительский узел текущего узла |
| [getStartIndex()](#getStartIndex--) | Получает начальный индекс символов. |
| [getTextOptions()](#getTextOptions--) | Возвращает параметры текста. |
| [getType()](#getType--) | Представляет тип узла. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Вставляет указанный узел после текущего узла. |
| [insertBefore(int equationType)](#insertBefore-int-) | Вставляет указанный узел перед текущим узлом. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Вставляет узел указанного типа в указанную позицию индекса в списке дочерних узлов текущего узла. |
| [isHideSubscript()](#isHideSubscript--) | Отображать нижнюю границу |
| [isHideSuperscript()](#isHideSuperscript--) | Отображать верхнюю границу |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Удаляет себя из родителя. |
| [removeAllChildren()](#removeAllChildren--) | Удаляет все дочерние узлы текущего узла. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Удаляет указанный узел из дочерних элементов текущего узла. |
| [removeChild(int index)](#removeChild-int-) | Удаляет узел с указанным индексом из дочерних элементов текущего узла. |
| [setHideSubscript(boolean value)](#setHideSubscript-boolean-) | Отображать нижнюю границу |
| [setHideSuperscript(boolean value)](#setHideSuperscript-boolean-) | Отображать верхнюю границу |
| [setLimitLocation(int value)](#setLimitLocation-int-) | Этот атрибут определяет расположение пределов в n-арных операторах. |
| [setNaryGrow(boolean value)](#setNaryGrow-boolean-) | Этот атрибут определяет свойство роста n-арных операторов на уровне документа. |
| [setNaryOperator(String value)](#setNaryOperator-java.lang.String-) | n-арный оператор, например "\u922d?. |
| [setNaryOperatorType(int value)](#setNaryOperatorType-int-) | n-арный оператор, например "\u922d? |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Указывает родительский узел текущего узла |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Устанавливает предустановленный стиль WordArt. |
| [toLaTeX()](#toLaTeX--) | Преобразуйте это уравнение в выражение LaTeX. |
| [toMathML()](#toMathML--) | Преобразуйте это уравнение в выражение MathML. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


Вставляет указанный узел в конец списка дочерних узлов текущего узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Указанный узел |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


Вставьте узел указанного типа в конец списка дочерних узлов текущего узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Типы узлов уравнения |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


Создайте узел указанного типа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Типы узлов уравнения |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Объект книги, связанный с уравнением |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | Родительский узел, в котором расположен этот узел |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Определите, равен ли текущий узел уравнения указанному узлу

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | Указанный узел |

**Returns:**
boolean -
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


Возвращает узел с указанным индексом среди дочерних узлов текущего узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс узла |

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


Получите тип уравнения текущего узла

Смотрите [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Возвращает шрифт этого объекта.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Получает длину символов.

**Returns:**
int
### getLimitLocation() {#getLimitLocation--}
```
public int getLimitLocation()
```


Этот атрибут указывает расположение пределов в n-арных операторах. Пределы могут быть либо центрированы над и под n-арным оператором, либо размещены сразу справа от оператора.

Смотрите [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Returns:**
int
### getNaryGrow() {#getNaryGrow--}
```
public boolean getNaryGrow()
```


Этот атрибут задает свойство роста n-арных операторов на уровне документа. Когда отключено, n-арные операторы, такие как интегралы и суммы, не увеличиваются, чтобы соответствовать высоте их операндов. Когда включено, n-арный оператор растет вертикально, чтобы соответствовать высоте его операнда.

**Returns:**
boolean
### getNaryOperator() {#getNaryOperator--}
```
public String getNaryOperator()
```


n-арный оператор, например "\\u922d?. Настоятельно рекомендуется использовать атрибут NaryOperatorType для установки n-арного оператора. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе.

**Remarks**

Следует отметить, что это свойство принимает только один символ, и если передано несколько символов, принимается только первый.

**Returns:**
java.lang.String
### getNaryOperatorType() {#getNaryOperatorType--}
```
public int getNaryOperatorType()
```


n-арный оператор, например "\u922d?

Смотрите [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Указывает родительский узел текущего узла

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Получает начальный индекс символов.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Возвращает параметры текста.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Представляет тип узла.

Смотрите [TextNodeType](../../com.aspose.cells/textnodetype).

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


Вставляет указанный узел после текущего узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Типы узлов уравнения |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


Вставляет указанный узел перед текущим узлом.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Типы узлов уравнения |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


Вставляет узел указанного типа в указанную позицию индекса в списке дочерних узлов текущего узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | значение индекса |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Типы узлов уравнения |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### isHideSubscript() {#isHideSubscript--}
```
public boolean isHideSubscript()
```


Отображать нижнюю границу

**Returns:**
boolean
### isHideSuperscript() {#isHideSuperscript--}
```
public boolean isHideSuperscript()
```


Отображать верхнюю границу

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


Удаляет себя из родителя.

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


Удаляет все дочерние узлы текущего узла.

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


Удаляет указанный узел из дочерних элементов текущего узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Узел, подлежащий удалению. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


Удаляет узел с указанным индексом из дочерних элементов текущего узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс узла |

### setHideSubscript(boolean value) {#setHideSubscript-boolean-}
```
public void setHideSubscript(boolean value)
```


Отображать нижнюю границу

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHideSuperscript(boolean value) {#setHideSuperscript-boolean-}
```
public void setHideSuperscript(boolean value)
```


Отображать верхнюю границу

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLimitLocation(int value) {#setLimitLocation-int-}
```
public void setLimitLocation(int value)
```


Этот атрибут указывает расположение пределов в n-арных операторах. Пределы могут быть либо центрированы над и под n-арным оператором, либо размещены сразу справа от оператора.

Смотрите [EquationLimitLocationType](../../com.aspose.cells/equationlimitlocationtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setNaryGrow(boolean value) {#setNaryGrow-boolean-}
```
public void setNaryGrow(boolean value)
```


Этот атрибут задает свойство роста n-арных операторов на уровне документа. Когда отключено, n-арные операторы, такие как интегралы и суммы, не увеличиваются, чтобы соответствовать высоте их операндов. Когда включено, n-арный оператор растет вертикально, чтобы соответствовать высоте его операнда.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNaryOperator(String value) {#setNaryOperator-java.lang.String-}
```
public void setNaryOperator(String value)
```


n-арный оператор, например "\\u922d?. Настоятельно рекомендуется использовать атрибут NaryOperatorType для установки n-арного оператора. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе.

**Remarks**

Следует отметить, что это свойство принимает только один символ, и если передано несколько символов, принимается только первый.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNaryOperatorType(int value) {#setNaryOperatorType-int-}
```
public void setNaryOperatorType(int value)
```


n-арный оператор, например "\u922d?

Смотрите [EquationMathematicalOperatorType](../../com.aspose.cells/equationmathematicaloperatortype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Указывает родительский узел текущего узла

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Устанавливает предустановленный стиль WordArt.

**Remarks**

Только для текста фигуры/диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Предустановленный стиль WordArt. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


Преобразуйте это уравнение в выражение LaTeX.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


Преобразуйте это уравнение в выражение MathML.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

