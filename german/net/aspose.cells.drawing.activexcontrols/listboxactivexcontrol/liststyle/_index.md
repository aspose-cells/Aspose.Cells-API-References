---
title: "ListBoxActiveXControl.ListStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBoxActiveXControl-Eigenschaft. Ruft das visuelle Erscheinungsbild ab und legt es fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/liststyle/
---
## ListBoxActiveXControl.ListStyle property

Liest und schreibt das visuelle Erscheinungsbild.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten für die ListBox hinzufügen
            sheet.Cells["A3"].Value = "Sales";
            sheet.Cells["A4"].Value = "Finance";
            sheet.Cells["A5"].Value = "MIS";
            sheet.Cells["A6"].Value = "R&D";
            sheet.Cells["A7"].Value = "Marketing";

            // Fügen Sie ein ListBox‑ActiveX‑Steuerelement hinzu
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Konfigurieren Sie die ListBox-Eigenschaften
            listBox.ListFillRange = "A3:A7";
            listBox.LinkedCell = "B1";
            listBox.ListStyle = ControlListStyle.Option; // Demonstrating ListStyle property
            listBox.SelectionType = SelectionType.Single;

            // Speichere die Arbeitsmappe
            workbook.Save("ListBoxActiveXControl_ListStyle_Demo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlListStyle](../../controlliststyle/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


