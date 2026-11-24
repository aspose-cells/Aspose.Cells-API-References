---
title: "ComboBoxActiveXControl.IsEditable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl property. Gibt an, ob der Benutzer in das Steuerelement tippen kann."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/iseditable/
---
## ComboBoxActiveXControl.IsEditable property

Gibt an, ob der Benutzer in das Steuerelement tippen kann.

```csharp
public bool IsEditable { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet sheet = workbook.Worksheets[0];

            // Füge ein ComboBox ActiveX-Steuerelement mithilfe der Shapes-Sammlung hinzu
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 5, 0, 100, 30);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Setze Eigenschaften für die ComboBox
            comboBox.IsEditable = true;
            comboBox.Value = "Editable ComboBox";
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 6;
            comboBox.TextColumn = 1;

            // Füge Elemente zur ComboBox hinzu (unter Verwendung der ListFillRange-Eigenschaft)
            sheet.Cells["A10"].PutValue("Item 1");
            sheet.Cells["B10"].PutValue("Description 1");
            sheet.Cells["A11"].PutValue("Item 2");
            sheet.Cells["B11"].PutValue("Description 2");
            comboBox.ListFillRange = "A10:B11";

            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxActiveXControl_IsEditableDemo.xlsx");

            // Eigenschaft nach dem Speichern überprüfen
            Console.WriteLine("IsEditable property value: " + comboBox.IsEditable);
        }
    }
}
```

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


