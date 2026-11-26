---
title: "TextBox.GetEquationParagraph"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TextBox. Получить указанный математический абзац из свойства TextBody объекта TextBox. Примечание 1 Возвращает NULL, когда индекс выходит за пределы или не найден. 2 Также возвращает NULL, если указанный индекс не является математическим абзацем"
type: docs
url: /ru/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

Получает указанный математический абзац из свойства TextBody объекта TextBox. Примечание: (1) Возвращает NULL, когда индекс выходит за пределы или не найден. (2) Также возвращает NULL, если указанная позиция индекса не является математическим абзацем.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс позиции математического абзаца, начиная с 0. |

### Возвращаемое значение

Возвращает математический абзац, указанный индексом.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class TextBoxMethodGetEquationParagraphWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Добавьте некоторое содержимое уравнения в текстовое поле
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // Вызовите GetEquationParagraph с параметром индекса (Int32)
                EquationNode equationNode = textBox.GetEquationParagraph(0);

                if (equationNode != null)
                {
                    Console.WriteLine("Equation paragraph retrieved successfully.");
                    Console.WriteLine($"Equation type: {equationNode.EquationType}");
                    Console.WriteLine($"LaTeX representation: {equationNode.ToLaTeX()}");
                }
                else
                {
                    Console.WriteLine("No equation paragraph found at the specified index.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEquationParagraph method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

Получает первый математический абзац из свойства TextBody объекта TextBox.

```csharp
public EquationNode GetEquationParagraph()
```

### Возвращаемое значение

Если есть математический абзац, возвращает первый, иначе возвращает null.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextBoxMethodGetEquationParagraphDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int textBoxIndex = worksheet.TextBoxes.Add(5, 5, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "$$\\sqrt{x^2+y^2}$$";
            
            EquationNode equationNode = textBox.GetEquationParagraph();
            
            if (equationNode != null)
            {
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                Console.WriteLine("Equation MathML: " + equationNode.ToMathML());
            }
            else
            {
                Console.WriteLine("No equation paragraph found");
            }
        }
    }
}
```

### См. также

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


