---
title: "Класс EquationNodeParagraph"
linktitle: "EquationNodeParagraph"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс EquationNodeParagraph. Инкапсулирует объект, представляющий equationnodeparagraph в Go."
type: docs
weight: 200
url: /ru/go-cpp/equationnodeparagraph/
---

## EquationNodeParagraph class

Этот класс определяет математический абзац, содержащий один или несколько элементов MathEquationNode(OMath).

```go

type EquationNodeParagraph struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewEquationNodeParagraph](./newequationnodeparagraph/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetJustification](./getjustification/) | Указывает выравнивание математического абзаца (серии смежных уравнений в одном абзаце). Математический абзац может быть выровнен по левому краю, по правому краю, по центру или центрирован как группа. По умолчанию математический абзац центрирован как группа. Это означает, что уравнения могут быть выровнены относительно друг друга, но вся группа уравнений центрируется в целом. |
| [SetJustification](./setjustification/) | Указывает выравнивание математического абзаца (серии смежных уравнений в одном абзаце). Математический абзац может быть выровнен по левому краю, по правому краю, по центру или центрирован как группа. По умолчанию математический абзац центрирован как группа. Это означает, что уравнения могут быть выровнены относительно друг друга, но вся группа уравнений центрируется в целом. |
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
| [EquationNodeParagraph_CreateNode](./equationnodeparagraph_createnode/) | Создайте узел указанного типа. |
