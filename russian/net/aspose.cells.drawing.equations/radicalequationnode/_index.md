---
title: "Класс RadicalEquationNode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Equations.RadicalEquationNode. Этот класс определяет радикальное уравнение, состоящее из необязательной степени degEquationNodeType.Degree и базы."
type: docs
url: /ru/net/aspose.cells.drawing.equations/radicalequationnode/
---
## RadicalEquationNode class

Этот класс определяет радикальное уравнение, состоящее из необязательной степени deg(EquationNodeType.Degree) и основания.

```csharp
public class RadicalEquationNode : EquationNode
```

## Свойства

| Имя | Описание |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Получить тип уравнения текущего узла (Унаследовано от [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Возвращает шрифт этого объекта (Унаследовано от [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsDegHide](../../aspose.cells.drawing.equations/radicalequationnode/isdeghide/) { get; set; } | Определяет, скрывать ли степень радикалов. |
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
| override [Equals](../../aspose.cells.drawing.equations/radicalequationnode/equals/)(object) | Определить, равен ли текущий узел уравнения указанному узлу |
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
    public class EquationsClassRadicalEquationNodeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить текстовое поле с уравнением на первый лист
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить узел уравнения
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Добавьте узел радикального уравнения
            RadicalEquationNode radicalNode = (RadicalEquationNode)mathNode.AddChild(EquationNodeType.Radical);
            radicalNode.IsDegHide = true;

            // Добавьте степень (скрытую) и базовые компоненты
            EquationNode degreeNode = radicalNode.AddChild(EquationNodeType.Degree);
            TextRunEquationNode degreeText = (TextRunEquationNode)degreeNode.AddChild(EquationNodeType.Text);
            degreeText.Text = "3";

            EquationNode baseNode = radicalNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x + 1";

            // Сохраните книгу
            workbook.Save("RadicalEquationDemo.xlsx");

            // Загрузите сохранённую книгу для проверки
            Workbook loadedWorkbook = new Workbook("RadicalEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            RadicalEquationNode loadedRadicalNode = (RadicalEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("Radical equation created successfully:");
            Console.WriteLine($"- IsDegHide: {loadedRadicalNode.IsDegHide}");
            Console.WriteLine($"- Base text: {((TextRunEquationNode)loadedRadicalNode.GetChild(1).GetChild(0)).Text}");
        }
    }
}
```

### См. также

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


