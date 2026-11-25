---
title: "ListBoxActiveXControl.ShowColumnHeads"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Indica se le intestazioni di colonna sono visualizzate"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/showcolumnheads/
---
## ListBoxActiveXControl.ShowColumnHeads property

Indica se le intestazioni di colonna sono visualizzate.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ListBox ActiveX con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ListBox, 
                1, 1, 100, 100,  // Left, Top, Width, Height
                0, 0);           // UpperLeftRow, UpperLeftColumn

            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il ListBox
            listBox.ColumnCount = 2;
            listBox.ListWidth = 150;
            listBox.ShowColumnHeads = true; // Demonstrate ShowColumnHeads property

            // Aggiungi alcuni dati di esempio
            listBox.Value = "Header1\tHeader2\nItem1\tData1\nItem2\tData2";

            // Salva la cartella di lavoro
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


