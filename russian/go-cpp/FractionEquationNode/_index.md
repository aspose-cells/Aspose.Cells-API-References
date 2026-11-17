---
title: "FractionEquationNode Класс"
linktitle: "FractionEquationNode"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "FractionEquationNode класс. Инкапсулирует объект, представляющий fractionequationnode в Go."
type: docs
weight: 200
url: /ru/go-cpp/fractionequationnode/
---

## FractionEquationNode class

Этот класс определяет уравнение дроби, состоящее из числителя и знаменателя, разделённых чертой дроби. Черта дроби может быть горизонтальной или диагональной, в зависимости от свойств дроби. Уравнение дроби также используется для представления функции стека, которая размещает один элемент над другим без черты дроби.

```go

type FractionEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewFractionEquationNode](./newfractionequationnode/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetFractionType](./getfractiontype/) | Это указывает тип дроби; значение по умолчанию — 'Bar'. |
| [SetFractionType](./setfractiontype/) | Это указывает тип дроби; значение по умолчанию — 'Bar'. |
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
| [FractionEquationNode_CreateNode](./fractionequationnode_createnode/) | Создайте узел указанного типа. |
