---
title: "Shape.FitToTextSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Пересчитать область текста, подходящую для отображения всего содержимого"
type: docs
url: /ru/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

Пересчитать область текста, подходящую для отображения всего содержимого.

```csharp
public void FitToTextSize()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeMethodFitToTextSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // Отобразить исходные размеры
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // Вызвать метод FitToTextSize
                textBox.FitToTextSize();

                // Отобразить скорректированные размеры
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // Добавьте больше текста, чтобы показать эффект
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


