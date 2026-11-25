---
title: "ComboBoxActiveXControl.BoundColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ComboBoxActiveXControl property. Rappresenta come la proprietà Value viene determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect è fmMultiSelectSingle"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/boundcolumn/
---
## ComboBoxActiveXControl.BoundColumn property

Rappresenta come la proprietà Value viene determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect è (fmMultiSelectSingle).

```csharp
public int BoundColumn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // Aggiungi un controllo ActiveX ComboBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 150, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Configura il ComboBox
            comboBox.ListFillRange = "A1:B4";
            comboBox.ColumnCount = 2;
            comboBox.BoundColumn = 0; // Bind to the ID column (column index 0)
            comboBox.TextColumn = 1; // Display the Name column (column index 1)

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ComboBox BoundColumn set to: " + comboBox.BoundColumn);
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


