---
title: "ListBoxActiveXControl.SelectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Indica se il controllo consente selezioni multiple"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/selectiontype/
---
## ListBoxActiveXControl.SelectionType property

Indica se il controllo consente selezioni multiple.

```csharp
public SelectionType SelectionType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Aggiungi il controllo ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà del ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            
            // Dimostra la proprietà SelectionType
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.Value = "Apple;Banana;Cherry";

            // Salva la cartella di lavoro
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");

            Console.WriteLine("ListBox with Single SelectionType created successfully.");
        }
    }
}
```

### Vedi anche

* enum [SelectionType](../../../aspose.cells.drawing/selectiontype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


