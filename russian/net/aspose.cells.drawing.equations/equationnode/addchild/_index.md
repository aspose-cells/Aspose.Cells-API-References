---
title: "EquationNode.AddChild"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Вставить узел указанного типа в конец списка дочерних узлов текущего узла"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/addchild/
---
## AddChild(EquationNodeType) {#addchild}

Вставить узел указанного типа в конец списка дочерних узлов текущего узла.

```csharp
public EquationNode AddChild(EquationNodeType equationType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| equationType | EquationNodeType | Типы узлов уравнения |

### Возвращаемое значение

Если указанный тип существует, возвращается соответствующий узел; если тип не существует, возвращается узел неизвестного типа.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodAddChildWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте форму уравнения на первый лист
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить корневой математический узел
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Создать узел функции и добавить дочерние элементы
            FunctionEquationNode functionNode = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);
            
            // Добавить имя функции с надстрочными символами
            EquationNode functionName = functionNode.AddChild(EquationNodeType.FunctionName);
            EquationNode supNode = functionName.AddChild(EquationNodeType.Sup);
            
            // Добавить базовый текст для имени функции
            EquationNode baseNode = supNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "Add";
            
            // Добавить надстрочный текст
            EquationNode superscriptNode = supNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscriptNode.AddChild(EquationNodeType.Text);
            superscriptText.Text = "-2";
            
            // Добавить аргумент функции
            EquationNode argumentNode = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argumentText = (TextRunEquationNode)argumentNode.AddChild(EquationNodeType.Text);
            argumentText.Text = "x";

            // Сохраните книгу
            workbook.Save("EquationNodeAddChildDemo.xlsx");
        }
    }
}
```

### См. также

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## AddChild(EquationNode) {#addchild_1}

Вставляет указанный узел в конец списка дочерних узлов текущего узла.

```csharp
public void AddChild(EquationNode node)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| узел | EquationNode | Указанный узел |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodAddChildWithEquationNodeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму уравнения
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Создать текстовый узел, который будет служить родителем
                var parentNode = equationNode.AddChild(EquationNodeType.Text);
                if (parentNode is TextRunEquationNode textNode)
                {
                    textNode.Text = "Parent Text";
                }

                // Создать дочерний узел для добавления с помощью статического метода CreateNode
                var childNode = EquationNode.CreateNode(EquationNodeType.Text, workbook, null);
                if (childNode is TextRunEquationNode childTextNode)
                {
                    childTextNode.Text = "Child Text";
                }

                // Вызвать метод AddChild с параметром EquationNode
                parentNode.AddChild(childNode);

                Console.WriteLine("AddChild method called successfully with EquationNode parameter");
                Console.WriteLine("Parent node has children: " + (parentNode.GetChild(0) != null));

                // Сохраните книгу
                workbook.Save("EquationNodeAddChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling AddChild: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


