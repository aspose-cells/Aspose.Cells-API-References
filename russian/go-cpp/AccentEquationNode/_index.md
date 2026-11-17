---
title: "Класс AccentEquationNode"
linktitle: "AccentEquationNode"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс AccentEquationNode. Инкапсулирует объект, представляющий accentequationnode в Go."
type: docs
weight: 200
url: /ru/go-cpp/accentequationnode/
---

## AccentEquationNode class

Этот класс определяет акцентное уравнение, состоящее из базового компонента и комбинирующего диакритического знака.

```go

type AccentEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewAccentEquationNode](./newaccentequationnode/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetAccentCharacter](./getaccentcharacter/) | Этот атрибут указывает тип комбинирующего диакритического знака, присоединяемого к основе функции акцента. Символ акцента по умолчанию — U+0302. Настоятельно рекомендуется использовать атрибут AccentType для установки символа акцента. Используйте эту настройку свойства, если вы не можете найти нужный символ в известном типе. |
| [SetAccentCharacter](./setaccentcharacter/) | Этот атрибут указывает тип комбинирующего диакритического знака, присоединяемого к основе функции акцента. Символ акцента по умолчанию — U+0302. Настоятельно рекомендуется использовать атрибут AccentType для установки символа акцента. Используйте эту настройку свойства, если вы не можете найти нужный символ в известном типе. |
| [GetAccentCharacterType](./getaccentcharactertype/) | Укажите комбинирующие символы по значению типа. |
| [SetAccentCharacterType](./setaccentcharactertype/) | Укажите комбинирующие символы по значению типа. |
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
| [AccentEquationNode_CreateNode](./accentequationnode_createnode/) | Создайте узел указанного типа. |
