---
title: "ComboBoxActiveXControl.SelectionMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Указывает, может ли пользователь выбрать строку текста, щелкнув в области слева от текста"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/selectionmargin/
---
## ComboBoxActiveXControl.SelectionMargin property

Указывает, может ли пользователь выбрать строку текста, щелкнув в области слева от текста.

```csharp
public bool SelectionMargin { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertySelectionMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрировать свойство SelectionMargin
            comboBox.SelectionMargin = false;
            Console.WriteLine("SelectionMargin set to: " + comboBox.SelectionMargin);

            // Переключить и снова продемонстрировать
            comboBox.SelectionMargin = true;
            Console.WriteLine("SelectionMargin now set to: " + comboBox.SelectionMargin);

            workbook.Save("ComboBoxSelectionMarginDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


