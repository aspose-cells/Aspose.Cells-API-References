---
title: "ListBoxActiveXControl.BoundColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Rappresenta come la proprietà Value è determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect è fmMultiSelectSingle"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/boundcolumn/
---
## ListBoxActiveXControl.BoundColumn property

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
    public class ListBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // Aggiungi il controllo ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 150, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà del ListBox
            listBox.ColumnCount = 2;
            listBox.ListFillRange = "A1:B4";
            
            // Imposta BoundColumn a 0 (colonna ID) - questo sarà il valore restituito quando un elemento è selezionato
            listBox.BoundColumn = 0;
            
            // Imposta TextColumn a 1 (colonna Nome) - questo verrà visualizzato nell'elenco
            listBox.TextColumn = 1;

            // Salva la cartella di lavoro
            workbook.Save("ListBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ListBox BoundColumn set to: " + listBox.BoundColumn);
        }
    }
}
```

### Vedi anche

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


