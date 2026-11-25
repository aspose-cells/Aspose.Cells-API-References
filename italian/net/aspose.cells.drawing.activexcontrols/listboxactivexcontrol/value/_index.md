---
title: "ListBoxActiveXControl.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Ottiene e imposta il valore del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/value/
---
## ListBoxActiveXControl.Value property

Ottiene e imposta il valore del controllo.

```csharp
public string Value { get; set; }
```

### Osservazioni

Ha effetto solo quando [`SelectionType`](../selectiontype/) è SelectionType.Single;

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà di base
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;

            // Imposta gli elementi usando la proprietà Value
            listBox.Value = "Red;Green;Blue;Yellow";

            // Salva la cartella di lavoro
            workbook.Save("ListBoxValueDemo.xlsx");

            Console.WriteLine("ListBox with items set using Value property has been created.");
        }
    }
}
```

### Vedi anche

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


