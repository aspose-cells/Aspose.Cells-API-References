---
title: "ComboBoxActiveXControl.ShowColumnHeads"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl-Eigenschaft. Gibt an, ob Spaltenüberschriften angezeigt werden"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showcolumnheads/
---
## ComboBoxActiveXControl.ShowColumnHeads property

Gibt an, ob Spaltenüberschriften angezeigt werden.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein ComboBox‑ActiveX‑Steuerelement hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Setze Eigenschaften für die ComboBox
            comboBox.ColumnCount = 2;
            comboBox.ListWidth = 100;
            
            // Beispieldaten zum ComboBox hinzufügen
            comboBox.ListFillRange = "A1:B3";
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("Value1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("Value2");

            // Demonstrieren Sie die ShowColumnHeads-Eigenschaft
            Console.WriteLine("Initial ShowColumnHeads value: " + comboBox.ShowColumnHeads);
            
            // Spaltenüberschriften aktivieren
            comboBox.ShowColumnHeads = true;
            Console.WriteLine("After setting ShowColumnHeads to true: " + comboBox.ShowColumnHeads);
            
            // Spaltenüberschriften deaktivieren
            comboBox.ShowColumnHeads = false;
            Console.WriteLine("After setting ShowColumnHeads to false: " + comboBox.ShowColumnHeads);

            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxShowColumnHeadsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


