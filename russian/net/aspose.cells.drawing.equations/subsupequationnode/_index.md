---
title: "Класс SubSupEquationNode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Equations.SubSupEquationNode. Этот класс определяет уравнение, которое может быть надстрочным или подстрочным. Существует четыре основных формы этого уравнения: надстрочный, подстрочный, надстрочный и подстрочный, размещённые слева от базового, и надстрочный и подстрочный, размещённые справа от базового."
type: docs
url: /ru/net/aspose.cells.drawing.equations/subsupequationnode/
---
## SubSupEquationNode class

Этот класс определяет уравнение, которое может быть надстрочным или подстрочным. Существует четыре основных формы этого уравнения: надстрочный, подстрочный, надстрочный и подстрочный, размещённые слева от основания, и надстрочный и подстрочный, размещённые справа от основания.

```csharp
public class SubSupEquationNode : EquationNode
```

## Свойства

| Имя | Описание |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Получить тип уравнения текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Возвращает шрифт этого объекта (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Получает длину символов (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Указывает родительский узел текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Получает начальный индекс символов (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Возвращает параметры текста (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Представляет тип узла (Унаследовано от [`EquationNode`](../equationnode/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Вставляет указанный узел в конец списка дочерних узлов текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Вставьте узел указанного типа в конец списка дочерних узлов текущего узла.(Наследовано от [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/subsupequationnode/equals/)(object) | Определить, равен ли текущий узел уравнения указанному узлу |
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
    public class EquationsClassSubSupEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            string[] vals = new string[] { "A", "B", "C" };

            // Создать подстрочное уравнение (A с подстрочным B)
            SubSupEquationNode subNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sub);
            AddBaseComponent(subNode, vals[0]);
            AddSubscriptComponent(subNode, vals[1]);

            // Создать надстрочное уравнение (A с надстрочным C)
            SubSupEquationNode supNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sup);
            AddBaseComponent(supNode, vals[0]);
            AddSuperscriptComponent(supNode, vals[2]);

            // Создать уравнение SubSup (A с подстрочным B и надстрочным C)
            SubSupEquationNode subSupNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.SubSup);
            AddBaseComponent(subSupNode, vals[0]);
            AddSubscriptComponent(subSupNode, vals[1]);
            AddSuperscriptComponent(subSupNode, vals[2]);

            // Создать уравнение PreSubSup (подстрочный B, надстрочный C, затем базовый A)
            SubSupEquationNode preSubSupNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.PreSubSup);
            AddSubscriptComponent(preSubSupNode, vals[1]);
            AddSuperscriptComponent(preSubSupNode, vals[2]);
            AddBaseComponent(preSubSupNode, vals[0]);

            workbook.Save("SubSupEquationDemo.xlsx");
        }

        private static void AddBaseComponent(SubSupEquationNode parent, string text)
        {
            EquationNode baseNode = parent.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }

        private static void AddSubscriptComponent(SubSupEquationNode parent, string text)
        {
            EquationNode subNode = parent.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode textNode = (TextRunEquationNode)subNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }

        private static void AddSuperscriptComponent(SubSupEquationNode parent, string text)
        {
            EquationNode supNode = parent.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode textNode = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }
    }
}
```

### См. также

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


