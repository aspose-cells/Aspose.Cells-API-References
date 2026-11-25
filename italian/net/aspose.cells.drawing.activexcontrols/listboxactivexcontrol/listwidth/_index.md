---
title: "ListBoxActiveXControl.ListWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Ottiene e imposta la larghezza in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/listwidth/
---
## ListBoxActiveXControl.ListWidth property

Ottiene e imposta la larghezza in unità di punti.

```csharp
public double ListWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ListBox ActiveX con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                10, 10, 200, 100, 200, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà ListWidth
            listBox.ListWidth = 150;
            
            // Configura le proprietà di base
            listBox.ColumnCount = 2;
            listBox.ColumnWidths = 100; // Changed from string to double
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Red");
            worksheet.Cells["B2"].PutValue("Yellow");
            worksheet.Cells["B3"].PutValue("Orange");
            
            // Imposta l'intervallo dei dati
            listBox.ListFillRange = "A1:B3";

            workbook.Save("ListBoxWidthDemo.xlsx");
            Console.WriteLine("ListBox with ListWidth=150 created successfully.");
        }
    }
}
```

### Vedi anche

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


