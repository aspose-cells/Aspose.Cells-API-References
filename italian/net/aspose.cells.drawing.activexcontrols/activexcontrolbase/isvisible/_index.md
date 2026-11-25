---
title: "ActiveXControlBase.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControlBase. Indica se questo controllo è visibile"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/
---
## ActiveXControlBase.IsVisible property

Indica se questo controllo è visibile.

```csharp
public virtual bool IsVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            var listBox = shape.ActiveXControl;

            // Configura le proprietà di base
            listBox.IsVisible = true; // Demonstrate IsVisible property
            Console.WriteLine("Initial visibility: " + listBox.IsVisible);
            listBox.IsVisible = false;
            Console.WriteLine("After setting to false: " + listBox.IsVisible);
            listBox.IsVisible = true;
            Console.WriteLine("After setting to true: " + listBox.IsVisible);

            // Salva la cartella di lavoro
            workbook.Save("ActiveXControlVisibilityDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


