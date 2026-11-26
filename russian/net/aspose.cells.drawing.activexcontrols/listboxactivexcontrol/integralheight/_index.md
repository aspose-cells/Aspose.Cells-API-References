---
title: "ListBoxActiveXControl.IntegralHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Указывает, будет ли элемент управления показывать только полные строки текста, без частичных строк"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/integralheight/
---
## ListBoxActiveXControl.IntegralHeight property

Указывает, будет ли элемент управления отображать только полные строки текста без частичных строк.

```csharp
public bool IntegralHeight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,
                10,  // left
                10,  // top
                200, // width
                100, // height
                0,   // imageWidth (required parameter)
                0    // imageHeight (required parameter)
            );
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрируйте свойство IntegralHeight
            listBox.IntegralHeight = true;
            Console.WriteLine("ListBox IntegralHeight set to: " + listBox.IntegralHeight);

            // Добавить примерные элементы
            listBox.ListFillRange = "A1:A3";
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            workbook.Save("ListBoxIntegralHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


