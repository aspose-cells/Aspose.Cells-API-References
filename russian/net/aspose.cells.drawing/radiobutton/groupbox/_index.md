---
title: "RadioButton.GroupBox"
second_title: "Справочник API Aspose.Cells для .NET"
description: "RadioButton свойство. Получает GroupBox, содержащий этот RadioButton"
type: docs
url: /ru/net/aspose.cells.drawing/radiobutton/groupbox/
---
## RadioButton.GroupBox property

Получает GroupBox, содержащий эту RadioButton.

```csharp
public GroupBox GroupBox { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonPropertyGroupBoxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить GroupBox для размещения RadioButton
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);
            groupBox.Name = "OptionsGroup";
            groupBox.Shadow = true;

            // Добавить RadioButton на лист (пока не в GroupBox)
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);

            // Отобразить начальные значения свойства GroupBox (должно быть null)
            Console.WriteLine("RadioButton1 GroupBox before grouping: " + (radioButton1.GroupBox == null ? "null" : radioButton1.GroupBox.Name));
            Console.WriteLine("RadioButton2 GroupBox before grouping: " + (radioButton2.GroupBox == null ? "null" : radioButton2.GroupBox.Name));

            // Добавить RadioButton в GroupBox, установив размещение
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;

            // Переместить RadioButton внутри GroupBox
            radioButton1.Top = groupBox.Top + 20;
            radioButton1.Left = groupBox.Left + 20;
            radioButton2.Top = groupBox.Top + 50;
            radioButton2.Left = groupBox.Left + 20;

            // Отобразить значения свойства GroupBox после группировки
            Console.WriteLine("RadioButton1 GroupBox after grouping: " + radioButton1.GroupBox.Name);
            Console.WriteLine("RadioButton2 GroupBox after grouping: " + radioButton2.GroupBox.Name);

            // Продемонстрировать поведение группы
            radioButton1.IsChecked = true;
            Console.WriteLine("RadioButton1 checked state: " + radioButton1.IsChecked);
            Console.WriteLine("RadioButton2 checked state: " + radioButton2.IsChecked);

            // Сохранить результат
            workbook.Save("RadioButtonPropertyGroupBoxDemo.xlsx");
        }
    }
}
```

### См. также

* class [GroupBox](../../groupbox/)
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


