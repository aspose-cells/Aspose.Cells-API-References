---
title: "ActiveXControlBase.ListFillRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControlBase. Получает и задает диапазон заполнения списка"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/
---
## ActiveXControlBase.ListFillRange property

Получает и задает диапазон заполнения списка.

```csharp
public string ListFillRange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyListFillRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для ListFillRange
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
            }

            // Добавьте ComboBoxActiveXControl
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1, 0, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Установите ListFillRange, чтобы заполнить combobox
            comboBox.ListFillRange = "A2:A10";

            // Сохраните книгу
            workbook.Save("ActiveXControlListFillRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


