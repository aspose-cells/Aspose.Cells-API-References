---
title: "DelimiterEquationNode Класс"
linktitle: "DelimiterEquationNode"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "DelimiterEquationNode класс. Инкапсулирует объект, представляющий delimiterequationnode в Go."
type: docs
weight: 200
url: /ru/go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

Этот класс определяет уравнение разделителя, состоящее из открывающих и закрывающих разделителей (таких как скобки, фигурные скобки, квадратные скобки и вертикальные черты) и содержащегося внутри компонента. Разделитель может иметь более одного компонента, с заданным символом‑разделителем между каждым компонентом.

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewDelimiterEquationNode](./newdelimiterequationnode/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetBeginChar](./getbeginchar/) | Символ начала разделителя. |
| [SetBeginChar](./setbeginchar/) | Символ начала разделителя. |
| [GetEndChar](./getendchar/) | Символ окончания разделителя. |
| [SetEndChar](./setendchar/) | Символ окончания разделителя. |
| [GetNaryGrow](./getnarygrow/) | Указывает, должен ли разделитель автоматически расширяться и сжиматься в зависимости от высоты формулы. |
| [SetNaryGrow](./setnarygrow/) | Указывает, должен ли разделитель автоматически расширяться и сжиматься в зависимости от высоты формулы. |
| [GetSeparatorChar](./getseparatorchar/) | Символ разделителя. |
| [SetSeparatorChar](./setseparatorchar/) | Символ разделителя. |
| [GetDelimiterShape](./getdelimitershape/) | Указывает форму разделителей в объекте разделителя. |
| [SetDelimiterShape](./setdelimitershape/) | Указывает форму разделителей в объекте разделителя. |
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
| [DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | Создайте узел указанного типа. |
