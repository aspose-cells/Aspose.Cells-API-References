---
title: "Класс DelimiterEquationNode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Equations.DelimiterEquationNode класс. Этот класс определяет уравнение разделителя, состоящее из открывающих и закрывающих разделителей, таких как скобки, фигурные скобки, квадратные скобки и вертикальные черты, а также содержащегося внутри компонента. Разделитель может иметь более одного компонента с указанным символом‑разделителем между каждым компонентом."
type: docs
url: /ru/net/aspose.cells.drawing.equations/delimiterequationnode/
---
## DelimiterEquationNode class

Этот класс определяет уравнение‑делимитер, состоящее из открывающих и закрывающих делимитеров (таких как скобки, фигурные скобки, квадратные скобки и вертикальные черты) и содержащегося внутри компонента. Делимитер может включать более одного компонента, с указанным разделительным символом между каждым компонентом.

```csharp
public class DelimiterEquationNode : EquationNode
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BeginChar](../../aspose.cells.drawing.equations/delimiterequationnode/beginchar/) { get; set; } | Символ начала разделителя. |
| [DelimiterShape](../../aspose.cells.drawing.equations/delimiterequationnode/delimitershape/) { get; set; } | Указывает форму разделителей в объекте разделителя. |
| [EndChar](../../aspose.cells.drawing.equations/delimiterequationnode/endchar/) { get; set; } | Символ окончания разделителя. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Получить тип уравнения текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Возвращает шрифт этого объекта (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Получает длину символов (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [NaryGrow](../../aspose.cells.drawing.equations/delimiterequationnode/narygrow/) { get; set; } | Указывает, должен ли разделитель автоматически расширяться и сжиматься в соответствии с высотой формулы. |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Указывает родительский узел текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [SeparatorChar](../../aspose.cells.drawing.equations/delimiterequationnode/separatorchar/) { get; set; } | Символ разделителя. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Получает начальный индекс символов (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Возвращает параметры текста (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Представляет тип узла (Унаследовано от [`EquationNode`](../equationnode/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Вставляет указанный узел в конец списка дочерних узлов текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Вставьте узел указанного типа в конец списка дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/delimiterequationnode/equals/)(object) | Определить, равен ли текущий узел уравнения указанному узлу |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Возвращает узел с указанным индексом среди дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Вставляет указанный узел после текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Вставляет указанный узел перед текущим узлом.(Наследовано от [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Вставляет узел указанного типа в указанную позицию индекса в список дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Удаляет себя из родителя.(Наследовано от [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Удаляет все дочерние узлы текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Удаляет указанный узел из дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Удаляет узел с указанным индексом из дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Устанавливает предустановленный стиль WordArt.(Наследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Преобразовать это уравнение в выражение LaTeX.(Наследовано от [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Преобразовать это уравнение в выражение MathML.(Наследовано от [`EquationNode`](../equationnode/).) |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassDelimiterEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Создать узел разделителя с пользовательскими настройками
            DelimiterEquationNode node = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            node.DelimiterShape = EquationDelimiterShapeType.Match;
            node.NaryGrow = false;
            node.SeparatorChar = "!";
            node.BeginChar = "#";
            node.EndChar = "*";

            // Добавить дробь в качестве базового содержимого
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            FractionEquationNode fraction = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);

            // Добавить числитель
            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textRun = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textRun.Text = "A";

            // Добавить знаменатель
            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            textRun = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textRun.Text = "B";

            // Добавить еще один базовый узел с текстом
            baseNode = node.AddChild(EquationNodeType.Base);
            textRun = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textRun.Text = "a";

            // Сохраните книгу
            workbook.Save("DelimiterEquationNodeDemo.xlsx");
        }
    }
}
```

### См. также

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


