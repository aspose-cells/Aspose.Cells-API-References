---
title: "EquationNode.InsertChild"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Вставляет узел указанного типа в указанную позицию индекса в список дочерних узлов текущего узла"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

Вставляет узел указанного типа в указанную позицию индекса в списке дочерних узлов текущего узла.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | значение индекса |
| equationType | EquationNodeType | Типы узлов уравнения |

### Возвращаемое значение

Если указанный тип существует, возвращается соответствующий узел; если тип не существует, возвращается узел неизвестного типа.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму уравнения
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Добавить начальный текстовый узел к уравнению
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // Вставить новый узел дроби в индекс 0
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // Сохраните книгу
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


