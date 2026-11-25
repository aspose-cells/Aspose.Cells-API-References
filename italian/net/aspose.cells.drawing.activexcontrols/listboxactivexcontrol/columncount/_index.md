---
title: "ListBoxActiveXControl.ColumnCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Rappresenta il numero di colonne da visualizzare in un ComboBox o ListBox"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columncount/
---
## ListBoxActiveXControl.ColumnCount property

Rappresenta il numero di colonne da visualizzare in un ComboBox o ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 1, 1, 1, 200, 100);
            var listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà includendo ColumnCount
            listBox.ColumnCount = 3;
            listBox.ListFillRange = "A1:C3"; // Sample data range for 3 columns

            // Verifica e visualizza il valore di ColumnCount
            Console.WriteLine("ListBox ColumnCount: " + listBox.ColumnCount);

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


