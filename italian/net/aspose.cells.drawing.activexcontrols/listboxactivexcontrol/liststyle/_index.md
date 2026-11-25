---
title: "ListBoxActiveXControl.ListStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Ottiene e imposta l'aspetto visivo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/liststyle/
---
## ListBoxActiveXControl.ListStyle property

Ottiene e imposta l'aspetto visivo.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyListStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la list box
            sheet.Cells["A3"].Value = "Sales";
            sheet.Cells["A4"].Value = "Finance";
            sheet.Cells["A5"].Value = "MIS";
            sheet.Cells["A6"].Value = "R&D";
            sheet.Cells["A7"].Value = "Marketing";

            // Aggiungi un controllo ActiveX ListBox
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà del ListBox
            listBox.ListFillRange = "A3:A7";
            listBox.LinkedCell = "B1";
            listBox.ListStyle = ControlListStyle.Option; // Demonstrating ListStyle property
            listBox.SelectionType = SelectionType.Single;

            // Salva la cartella di lavoro
            workbook.Save("ListBoxActiveXControl_ListStyle_Demo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlListStyle](../../controlliststyle/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


