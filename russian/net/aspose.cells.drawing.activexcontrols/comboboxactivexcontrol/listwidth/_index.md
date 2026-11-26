---
title: "ComboBoxActiveXControl.ListWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Получает и задает ширину в единицах пунктов"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listwidth/
---
## ComboBoxActiveXControl.ListWidth property

Получает и задает ширину в единицах пунктов.

```csharp
public double ListWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для ComboBox
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            // Добавить элемент управления ComboBox ActiveX со всеми необходимыми параметрами
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1,  // left
                1,  // top
                100, // width
                30,  // height
                0,   // image width (unused for ComboBox)
                0    // image height (unused for ComboBox)
            );
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Установить свойство ListWidth для управления шириной выпадающего списка
            comboBox.ListWidth = 150;
            comboBox.ListRows = 3;
            comboBox.LinkedCell = "A1:A3";

            // Сохраните книгу
            workbook.Save("ComboBoxListWidthDemo.xlsx");

            Console.WriteLine("ComboBox ListWidth set to: " + comboBox.ListWidth);
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


