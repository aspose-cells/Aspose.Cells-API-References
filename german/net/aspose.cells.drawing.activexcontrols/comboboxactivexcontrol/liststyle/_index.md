---
title: "ComboBoxActiveXControl.ListStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl Eigenschaft. Liest und setzt das visuelle Erscheinungsbild"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/liststyle/
---
## ComboBoxActiveXControl.ListStyle property

Liest und schreibt das visuelle Erscheinungsbild.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Items");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");

            // ComboBox mit einfachem Listenstil hinzufügen
            var comboBoxShape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
            comboBox.ListStyle = Aspose.Cells.Drawing.ActiveXControls.ControlListStyle.Plain;
            comboBox.ListFillRange = "A2:A4";

            // ListBox mit Optionslistenstil hinzufügen
            var listBoxShape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)listBoxShape.ActiveXControl;
            listBox.ListStyle = Aspose.Cells.Drawing.ActiveXControls.ControlListStyle.Option;
            listBox.ListFillRange = "A2:A4";

            // Speichern und demonstrieren
            workbook.Save("ListStyleDemo.xlsx");
            Console.WriteLine("ComboBox ListStyle: " + comboBox.ListStyle);
            Console.WriteLine("ListBox ListStyle: " + listBox.ListStyle);
        }
    }
}
```

### Siehe auch

* enum [ControlListStyle](../../controlliststyle/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


