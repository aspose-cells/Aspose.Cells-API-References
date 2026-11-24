---
title: "ComboBoxActiveXControl.BoundColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl property. Gibt an, wie die Value-Eigenschaft für eine ComboBox oder ListBox bestimmt wird, wenn der Wert der MultiSelect-Eigenschaft fmMultiSelectSingle ist."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/boundcolumn/
---
## ComboBoxActiveXControl.BoundColumn property

Beschreibt, wie die Value-Eigenschaft für ein ComboBox- oder ListBox-Steuerelement bestimmt wird, wenn der Wert der MultiSelect-Eigenschaft (fmMultiSelectSingle) ist.

```csharp
public int BoundColumn { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // Ein ComboBox‑ActiveX‑Steuerelement hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 150, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // ComboBox konfigurieren
            comboBox.ListFillRange = "A1:B4";
            comboBox.ColumnCount = 2;
            comboBox.BoundColumn = 0; // Bind to the ID column (column index 0)
            comboBox.TextColumn = 1; // Display the Name column (column index 1)

            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ComboBox BoundColumn set to: " + comboBox.BoundColumn);
        }
    }
}
```

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


