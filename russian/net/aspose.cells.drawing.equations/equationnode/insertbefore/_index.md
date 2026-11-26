---
title: "EquationNode.InsertBefore"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Вставляет указанный узел перед текущим узлом"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/insertbefore/
---
## EquationNode.InsertBefore method

Вставляет указанный узел перед текущим узлом.

```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
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

    public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте математическое уравнение в ячейке A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Добавить начальный текстовый узел к уравнению
            var textNode = equationNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

            try
            {
                // Вставьте новый текстовый узел перед существующим
                var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
                
                // Отобразите уравнение в формате LaTeX
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


