---
title: "Класс SubSupEquationNode"
linktitle: "SubSupEquationNode"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс SubSupEquationNode. Инкапсулирует объект, представляющий subsupequationnode в Go."
type: docs
weight: 200
url: /ru/go-cpp/subsupequationnode/
---

## SubSupEquationNode class

Этот класс определяет уравнение, которое может быть в виде надстрочного или подстрочного индекса. Существует четыре основных формы этого уравнения: надстрочный, подстрочный, надстрочный и подстрочный, размещённые слева от основания, и надстрочный и подстрочный, размещённые справа от основания.

```go

type SubSupEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewSubSupEquationNode](./newsubsupequationnode/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
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
| [SubSupEquationNode_CreateNode](./subsupequationnode_createnode/) | Создайте узел указанного типа. |
