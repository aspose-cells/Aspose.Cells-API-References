---
title: "ListBoxActiveXControl.BoundColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBoxActiveXControl-Eigenschaft. Gibt an, wie die Value-Eigenschaft für ein ComboBox oder ListBox bestimmt wird, wenn der Wert der MultiSelect-Eigenschaft fmMultiSelectSingle ist."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/boundcolumn/
---
## ListBoxActiveXControl.BoundColumn property

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
    public class ListBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // ListBox ActiveX-Steuerelement hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 150, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // ListBox-Eigenschaften konfigurieren
            listBox.ColumnCount = 2;
            listBox.ListFillRange = "A1:B4";
            
            // Setze BoundColumn auf 0 (ID-Spalte) – dies wird der zurückgegebene Wert sein, wenn ein Element ausgewählt wird.
            listBox.BoundColumn = 0;
            
            // Setze TextColumn auf 1 (Namensspalte) – dies wird in der Liste angezeigt.
            listBox.TextColumn = 1;

            // Speichere die Arbeitsmappe
            workbook.Save("ListBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ListBox BoundColumn set to: " + listBox.BoundColumn);
        }
    }
}
```

### Siehe auch

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


