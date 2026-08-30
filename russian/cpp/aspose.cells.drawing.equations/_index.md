---
title: Пространство имён Aspose::Cells::Drawing::Equations
linktitle: Aspose::Cells::Drawing::Equations
second_title: Справочник API Aspose.Cells для C++
description: 'Как использовать пространство имён Aspose::Cells::Drawing::Equations в C++.'
type: docs
weight: 600
url: /ru/cpp/aspose.cells.drawing.equations/
---



## Классы

| Класс | Описание |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | Этот класс задаёт акцентное уравнение, состоящее из базового компонента и комбинирующего диакритического знака. |
| [ArrayEquationNode](./arrayequationnode/) | Задаёт функцию Equation-Array, объект, состоящий из одного или нескольких уравнений. |
| [BarEquationNode](./barequationnode/) | Этот класс задаёт бар‑уравнение, состоящее из базового аргумента и надчерты или подчерты. |
| [BorderBoxEquationNode](./borderboxequationnode/) | Этот класс задаёт функцию [Border](../aspose.cells/border/) Box, состоящую из границы, нарисованной вокруг уравнения. |
| [BoxEquationNode](./boxequationnode/) | Этот класс задаёт функцию box, которая используется для группировки компонентов уравнения. |
| [DelimiterEquationNode](./delimiterequationnode/) | Этот класс задаёт уравнение‑делимитер, состоящее из открывающих и закрывающих делимитеров (например, скобок, фигурных скобок, квадратных скобок и вертикальных черт) и содержащегося внутри компонента. Делимитер может иметь более одного компонента, между которыми находится указанный разделительный символ. |
| [EquationComponentNode](./equationcomponentnode/) | Этот класс задаёт компоненты уравнения или математического выражения. Разные типы компонентов комбинируются в разные уравнения. Например, дробь состоит из двух частей: числителя и знаменателя. Для получения информации о дополнительных типах компонентов см. 'EquationNodeType'. |
| [EquationNode](./equationnode/) | Абстрактный класс для создания других узлов уравнений. |
| [EquationNodeParagraph](./equationnodeparagraph/) | Этот класс определяет математический абзац, содержащий один или несколько элементов MathEquationNode(OMath). |
| [FractionEquationNode](./fractionequationnode/) | Этот класс определяет дробное уравнение, состоящее из числителя и знаменателя, разделённых чертой дроби. Черта дроби может быть горизонтальной или диагональной, в зависимости от свойств дроби. Дробное уравнение также используется для представления функции stack, которая размещает один элемент над другим без черты дроби. |
| [FunctionEquationNode](./functionequationnode/) | Этот класс определяет уравнение Function-Apply, которое состоит из имени функции и аргумента, к которому применяется действие. Типы компонентов имени и аргумента соответственно являются '[EquationNodeType.FunctionName](./equationnodetype/)' и '[EquationNodeType.Base](./equationnodetype/)'. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | Этот класс определяет функцию Group-Character, состоящую из символа, размещённого над или под текстом, часто с целью визуального группирования элементов. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | Этот класс определяет функцию предела. |
| [MathematicalEquationNode](./mathematicalequationnode/) | Этот класс определяет уравнение или математическое выражение. Весь математический текст уравнений или математических выражений содержится в этом классе. |
| [MatrixEquationNode](./matrixequationnode/) | Этот класс определяет матричное уравнение, состоящее из одного или нескольких элементов, расположенных в одной или нескольких строках и одной или нескольких колонках. |
| [NaryEquationNode](./naryequationnode/) | Этот класс определяет n-арное операторное уравнение, состоящее из n-арного оператора, основания (или операнда) и необязательных верхних и нижних границ. |
| [RadicalEquationNode](./radicalequationnode/) | Этот класс определяет радикальное уравнение, состоящее из необязательной степени deg([EquationNodeType.Degree](./equationnodetype/)) и основания. |
| [SubSupEquationNode](./subsupequationnode/) | Этот класс определяет уравнение, которое может быть надстрочным или подстрочным по желанию. Существует четыре основных формы этого уравнения: надстрочный, подстрочный, надстрочный и подстрочный, размещённые слева от основания, и надстрочный и подстрочный, размещённые справа от основания. |
| [TextRunEquationNode](./textrunequationnode/) | Этот класс в узле уравнения используется для хранения фактического содержимого (последовательности математического текста) уравнения. Обычно создаётся объект узла для каждого символа. |
| [UnknowEquationNode](./unknowequationnode/) | Класс узла уравнения неизвестного типа. |
## Enums

| Перечисление | Описание |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | Определяет позицию конкретного подобъекта внутри его родителя. |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | Тип комбинирующих символов. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | Это определяет форму разделителей в объекте разделителя. |
| [EquationFractionType](./equationfractiontype/) | Это определяет стиль отображения черты дроби. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | Это определяет горизонтальное выравнивание уравнений в документе по умолчанию. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | Определяет расположение предела над оператором. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | Тип математических операторов. |
| [EquationNodeType](./equationnodetype/) | Тип узла уравнения. Примечание: (1)[1-99] В текущей области присутствует только один узел, его перечислимое значение равно 1. Указанный узел используется для хранения математического текста. (2)[100-199] Указывает, что узел является компонентом некоторых специальных узлов функций. (3)[200-] Указывает, что у узла есть некоторые специальные функции. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | Это определяет вертикальное выравнивание уравнений в документе по умолчанию. |
