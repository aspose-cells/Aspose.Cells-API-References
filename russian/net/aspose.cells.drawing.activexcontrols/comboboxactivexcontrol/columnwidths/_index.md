---
title: "ComboBoxActiveXControl.ColumnWidths"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Получает и задает ширину столбца"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columnwidths/
---
## ComboBoxActiveXControl.ColumnWidths property

Получает и задает ширину столбца.

```csharp
public double ColumnWidths { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyColumnWidthsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                5, 0, 100, 20, 100, 20);
            
            var comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            comboBox.ColumnCount = 3;
            comboBox.ListRows = 5;
            
            // Установите ширину столбцов (используя двойное значение для ширины одного столбца)
            comboBox.ColumnWidths = 100;

            // Установите элементы списка через ListFillRange
            worksheet.Cells["A1"].PutValue("Product\tPrice\tStock");
            worksheet.Cells["A2"].PutValue("Laptop\t$999\t50");
            worksheet.Cells["A3"].PutValue("Phone\t$699\t120");
            worksheet.Cells["A4"].PutValue("Tablet\t$399\t75");
            comboBox.ListFillRange = "A1:A4";

            workbook.Save("ComboBoxColumnWidthsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


