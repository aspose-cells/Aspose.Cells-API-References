---
title: "Класс NaryEquationNode"
linktitle: "NaryEquationNode"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс NaryEquationNode. Инкапсулирует объект, представляющий naryequationnode в Go."
type: docs
weight: 200
url: /ru/go-cpp/naryequationnode/
---

## NaryEquationNode class

Этот класс определяет n-арное операторное уравнение, состоящее из n-арного оператора, основания (или операнда) и необязательных верхних и нижних границ.

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewNaryEquationNode](./newnaryequationnode/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [IsHideSubscript](./ishidesubscript/) | Отображать ли нижнюю границу |
| [SetIsHideSubscript](./setishidesubscript/) | Отображать ли нижнюю границу |
| [IsHideSuperscript](./ishidesuperscript/) | Отображать ли верхнюю границу |
| [SetIsHideSuperscript](./setishidesuperscript/) | Отображать ли верхнюю границу |
| [GetLimitLocation](./getlimitlocation/) | Этот атрибут указывает расположение пределов в n-арных операторах. Пределы могут быть либо центрированы над и под n-арным оператором, либо расположены сразу справа от оператора. |
| [SetLimitLocation](./setlimitlocation/) | Этот атрибут указывает расположение пределов в n-арных операторах. Пределы могут быть либо центрированы над и под n-арным оператором, либо расположены сразу справа от оператора. |
| [GetNaryOperator](./getnaryoperator/) | n-арный оператор, например "∑". Настоятельно рекомендуется использовать атрибут NaryOperatorType для установки n-арного оператора. Используйте эту настройку свойства, если вы не можете найти нужный символ в известном типе. |
| [SetNaryOperator](./setnaryoperator/) | n-арный оператор, например "∑". Настоятельно рекомендуется использовать атрибут NaryOperatorType для установки n-арного оператора. Используйте эту настройку свойства, если вы не можете найти нужный символ в известном типе. |
| [GetNaryOperatorType](./getnaryoperatortype/) | n-арный оператор, например "∑" |
| [SetNaryOperatorType](./setnaryoperatortype/) | n-арный оператор, например "∑" |
| [GetNaryGrow](./getnarygrow/) | Этот атрибут указывает свойство роста n-арных операторов на уровне документа. Когда отключено, n-арные операторы, такие как интегралы и суммы, не увеличиваются, чтобы соответствовать высоте их операндов. Когда включено, n-арный оператор растёт вертикально, чтобы соответствовать высоте своего операнда. |
| [SetNaryGrow](./setnarygrow/) | Этот атрибут указывает свойство роста n-арных операторов на уровне документа. Когда отключено, n-арные операторы, такие как интегралы и суммы, не увеличиваются, чтобы соответствовать высоте их операндов. Когда включено, n-арный оператор растёт вертикально, чтобы соответствовать высоте своего операнда. |
| [Equals](./equals/) | Определите, равен ли текущий узел уравнения указанному узлу |
| [GetStartIndex](./getstartindex/) | Получает начальный индекс символов. |
| [GetLength](./getlength/) | Получает длину символов. |
| [GetFont](./getfont/) | Возвращает шрифт этого объекта. |
| [SetWordArtStyle](./setwordartstyle/) | Устанавливает предустановленный стиль WordArt. |
| [GetTextOptions](./gettextoptions/) | Возвращает параметры текста. |
| [GetType](./gettype/) | Получает тип текстового узла. |
| [GetParentNode](./getparentnode/) | Указывает родительский узел текущего узла |
| [SetParentNode](./setparentnode/) | Указывает родительский узел текущего узла |
| [ToLaTeX](./tolatex/) | Преобразуйте это уравнение в выражение LaTeX. |
| [ToMathML](./tomathml/) | Преобразуйте это уравнение в выражение MathML. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | Вставьте узел указанного типа в конец списка дочерних узлов текущего узла. |
| [InsertChild](./insertchild/) | Вставляет узел указанного типа в указанную позицию индекса в списке дочерних узлов текущего узла. |
| [InsertAfter](./insertafter/) | Вставляет указанный узел после текущего узла. |
| [InsertBefore](./insertbefore/) | Вставляет указанный узел перед текущим узлом. |
| [GetChild](./getchild/) | Возвращает узел с указанным индексом среди дочерних узлов текущего узла. |
| [Remove](./remove/) | Удаляет себя из родителя. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | Удаляет указанный узел из дочерних узлов текущего узла. |
| [RemoveAllChildren](./removeallchildren/) | Удаляет все дочерние узлы текущего узла. |
| [GetEquationType](./getequationtype/) | Получите тип уравнения текущего узла |
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | Создайте узел указанного типа. |
