---
title: "MatrixEquationNode"
second_title: "Справочник API Aspose.Cells for Java"
description: "Этот класс определяет уравнение Matrix, состоящее из одного или нескольких элементов, расположенных в одной или нескольких строках и одной или нескольких колонках."
type: docs
url: /ru/java/com.aspose.cells/matrixequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class MatrixEquationNode extends EquationNode
```

Этот класс определяет матричное уравнение, состоящее из одного или нескольких элементов, расположенных в одной или нескольких строках и одной или нескольких колонках.
## Методы

| Метод | Описание |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Вставляет указанный узел в конец списка дочерних узлов текущего узла. |
| [addChild(int equationType)](#addChild-int-) | Вставьте узел указанного типа в конец списка дочерних узлов текущего узла. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Создайте узел указанного типа. |
| [equals(Object obj)](#equals-java.lang.Object-) | Определите, равен ли текущий узел уравнения указанному узлу |
| [getBaseJc()](#getBaseJc--) | Этот атрибут задаёт выравнивание матрицы. |
| [getChild(int index)](#getChild-int-) | Возвращает узел с указанным индексом среди дочерних узлов текущего узла. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Получите тип уравнения текущего узла |
| [getFont()](#getFont--) | Возвращает шрифт этого объекта. |
| [getLength()](#getLength--) | Получает длину символов. |
| [getParentNode()](#getParentNode--) | Указывает родительский узел текущего узла |
| [getStartIndex()](#getStartIndex--) | Получает начальный индекс символов. |
| [getTextOptions()](#getTextOptions--) | Возвращает параметры текста. |
| [getType()](#getType--) | Представляет тип узла. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Вставляет указанный узел после текущего узла. |
| [insertBefore(int equationType)](#insertBefore-int-) | Вставляет указанный узел перед текущим узлом. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Вставляет узел указанного типа в указанную позицию индекса в списке дочерних узлов текущего узла. |
| [isHidePlaceholder()](#isHidePlaceholder--) | Этот атрибут задаёт свойство Hide Placeholders для матрицы. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Удаляет себя из родителя. |
| [removeAllChildren()](#removeAllChildren--) | Удаляет все дочерние узлы текущего узла. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Удаляет указанный узел из дочерних элементов текущего узла. |
| [removeChild(int index)](#removeChild-int-) | Удаляет узел с указанным индексом из дочерних элементов текущего узла. |
| [setBaseJc(int value)](#setBaseJc-int-) | Этот атрибут задаёт выравнивание матрицы. |
| [setHidePlaceholder(boolean value)](#setHidePlaceholder-boolean-) | Этот атрибут задаёт свойство Hide Placeholders для матрицы. |
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
### getBaseJc() {#getBaseJc--}
```
public int getBaseJc()
```


Этот атрибут задаёт выравнивание матрицы. Текст за пределами матрицы может быть выровнен по нижнему, верхнему или центральному краю функции матрицы. По умолчанию матрица использует центральное выравнивание.

См. [EquationVerticalJustificationType](../../com.aspose.cells/equationverticaljustificationtype).

**Returns:**
int
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
### isHidePlaceholder() {#isHidePlaceholder--}
```
public boolean isHidePlaceholder()
```


Этот атрибут задаёт свойство Hide Placeholders для матрицы. Когда это свойство включено, заполнители не отображаются в матрице. По умолчанию заполнители отображаются, делая видимыми места, куда можно вставить текст.

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

### setBaseJc(int value) {#setBaseJc-int-}
```
public void setBaseJc(int value)
```


Этот атрибут задаёт выравнивание матрицы. Текст за пределами матрицы может быть выровнен по нижнему, верхнему или центральному краю функции матрицы. По умолчанию матрица использует центральное выравнивание.

См. [EquationVerticalJustificationType](../../com.aspose.cells/equationverticaljustificationtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHidePlaceholder(boolean value) {#setHidePlaceholder-boolean-}
```
public void setHidePlaceholder(boolean value)
```


Этот атрибут задаёт свойство Hide Placeholders для матрицы. Когда это свойство включено, заполнители не отображаются в матрице. По умолчанию заполнители отображаются, делая видимыми места, куда можно вставить текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

