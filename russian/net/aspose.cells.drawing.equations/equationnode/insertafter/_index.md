---
title: "EquationNode.InsertAfter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Вставляет указанный узел после текущего узла"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

Вставляет указанный узел после текущего узла.

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
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

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте форму уравнения в ячейке A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Добавьте начальный текстовый узел
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // Вставьте новый текстовый узел после существующего
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // Отобразите структуру уравнения
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // Сохраните уравнение в ячейку для визуального осмотра
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### См. также

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


