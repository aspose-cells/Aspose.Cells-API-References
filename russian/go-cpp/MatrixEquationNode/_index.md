---
title: "MatrixEquationNode Класс"
linktitle: "MatrixEquationNode"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "MatrixEquationNode класс. Инкапсулирует объект, представляющий matrixequationnode в Go."
type: docs
weight: 200
url: /ru/go-cpp/matrixequationnode/
---

## MatrixEquationNode class

Этот класс определяет матричное уравнение, состоящее из одного или нескольких элементов, расположенных в одной или нескольких строках и одной или нескольких колонках.

```go

type MatrixEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewMatrixEquationNode](./newmatrixequationnode/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetBaseJc](./getbasejc/) | Этот атрибут задает выравнивание матрицы. Текст за пределами матрицы может быть выровнен по нижнему, верхнему или центральному краю функции матрицы. По умолчанию матрица использует центральное выравнивание. |
| [SetBaseJc](./setbasejc/) | Этот атрибут задает выравнивание матрицы. Текст за пределами матрицы может быть выровнен по нижнему, верхнему или центральному краю функции матрицы. По умолчанию матрица использует центральное выравнивание. |
| [IsHidePlaceholder](./ishideplaceholder/) | Этот атрибут задает свойство Hide Placeholders для матрицы. Когда это свойство включено, заполнители не отображаются в матрице. По умолчанию заполнители отображаются, делая видимыми места, куда можно вставить текст. |
| [SetIsHidePlaceholder](./setishideplaceholder/) | Этот атрибут задает свойство Hide Placeholders для матрицы. Когда это свойство включено, заполнители не отображаются в матрице. По умолчанию заполнители отображаются, делая видимыми места, куда можно вставить текст. |
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
| [MatrixEquationNode_CreateNode](./matrixequationnode_createnode/) | Создайте узел указанного типа. |
