---
title: "RadioButton.GetOptionIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод RadioButton. Получает индекс опции, начинающийся с 1, среди всех радиокнопок GroupBox, содержащего эту радиокнопку"
type: docs
url: /ru/net/aspose.cells.drawing/radiobutton/getoptionindex/
---
## RadioButton.GetOptionIndex method

Получает индекс опции (нумерация с единицы) среди всех радиокнопок GroupBox, содержащих эту радиокнопку.

```csharp
public int GetOptionIndex()
```

### Примечания

Если эта радиокнопка не находится в GroupBox, возвращает индекс опции среди всех радиокнопок, которые не находятся ни в одном GroupBox

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonMethodGetOptionIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить GroupBox для размещения RadioButton
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);

            // Добавить три радиокнопки в GroupBox
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);
            RadioButton radioButton3 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 80, 100, 20, 100);

            // Установить радиокнопки как часть GroupBox
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;
            radioButton3.Placement = PlacementType.FreeFloating;

            try
            {
                // Получить индекс опции для каждой радиокнопки
                int index1 = radioButton1.GetOptionIndex();
                int index2 = radioButton2.GetOptionIndex();
                int index3 = radioButton3.GetOptionIndex();

                Console.WriteLine($"RadioButton1 Option Index: {index1}");
                Console.WriteLine($"RadioButton2 Option Index: {index2}");
                Console.WriteLine($"RadioButton3 Option Index: {index3}");

                // Отметить первую радиокнопку, чтобы продемонстрировать выбор
                radioButton1.IsChecked = true;
                Console.WriteLine("RadioButton1 is checked");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOptionIndex method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("RadioButtonMethodGetOptionIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


