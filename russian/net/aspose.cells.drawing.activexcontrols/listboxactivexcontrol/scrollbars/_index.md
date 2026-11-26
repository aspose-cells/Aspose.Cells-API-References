---
title: "ListBoxActiveXControl.ScrollBars"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные полосы прокрутки, оба или ни одного"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/scrollbars/
---
## ListBoxActiveXControl.ScrollBars property

Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные, обе или ни одну.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBoxControl = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Добавьте несколько элементов, чтобы полосы прокрутки стали видимыми
            listBoxControl.ListFillRange = "A1:A20";
            for (int i = 1; i <= 20; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }

            // Продемонстрировать свойство ScrollBars
            listBoxControl.ScrollBars = Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType.BarsBoth;

            workbook.Save("ListBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


