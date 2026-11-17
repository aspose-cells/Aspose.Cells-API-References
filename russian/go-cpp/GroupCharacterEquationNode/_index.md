---
title: "Класс GroupCharacterEquationNode"
linktitle: "GroupCharacterEquationNode"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс GroupCharacterEquationNode. Инкапсулирует объект, представляющий groupcharacterequationnode в Go."
type: docs
weight: 200
url: /ru/go-cpp/groupcharacterequationnode/
---

## GroupCharacterEquationNode class

Этот класс определяет функцию группировки символов, состоящую из символа, размещённого над или под текстом, часто с целью визуального объединения элементов.

```go

type GroupCharacterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewGroupCharacterEquationNode](./newgroupcharacterequationnode/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetGroupChr](./getgroupchr/) | Указывает символ (по умолчанию U+23DF). Настоятельно рекомендуется использовать атрибут ChrType для установки акцентного символа. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе. |
| [SetGroupChr](./setgroupchr/) | Указывает символ (по умолчанию U+23DF). Настоятельно рекомендуется использовать атрибут ChrType для установки акцентного символа. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе. |
| [GetChrType](./getchrtype/) | Укажите комбинирующие символы по значению типа. |
| [SetChrType](./setchrtype/) | Укажите комбинирующие символы по значению типа. |
| [GetPosition](./getposition/) | Этот атрибут указывает позицию символа в объекте |
| [SetPosition](./setposition/) | Этот атрибут указывает позицию символа в объекте |
| [GetVertJc](./getvertjc/) | Этот атрибут в сочетании с pos из groupChrPr определяет вертикальное расположение объекта groupChr. Где pos указывает позицию группирующего символа, vertJc определяет выравнивание объекта относительно базовой линии. |
| [SetVertJc](./setvertjc/) | Этот атрибут в сочетании с pos из groupChrPr определяет вертикальное расположение объекта groupChr. Где pos указывает позицию группирующего символа, vertJc определяет выравнивание объекта относительно базовой линии. |
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
| [GroupCharacterEquationNode_CreateNode](./groupcharacterequationnode_createnode/) | Создайте узел указанного типа. |
