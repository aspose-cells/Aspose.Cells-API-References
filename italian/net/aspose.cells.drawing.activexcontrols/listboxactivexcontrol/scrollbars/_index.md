---
title: "ListBoxActiveXControl.ScrollBars"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/scrollbars/
---
## ListBoxActiveXControl.ScrollBars property

Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Esempi

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

            // Aggiungi alcuni elementi per rendere visibili le barre di scorrimento
            listBoxControl.ListFillRange = "A1:A20";
            for (int i = 1; i <= 20; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }

            // Dimostra la proprietà ScrollBars
            listBoxControl.ScrollBars = Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType.BarsBoth;

            workbook.Save("ListBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


