---
title: "ActiveXControlBase.Data"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Liest und schreibt die Binärdaten des Steuerelements"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/data/
---
## ActiveXControlBase.Data property

Liest und setzt die Binärdaten des Steuerelements.

```csharp
public virtual byte[] Data { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;
    using System.Drawing;

    public class ActiveXControlBasePropertyDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            shape.Name = "MyList";
            ListBoxActiveXControl list = (ListBoxActiveXControl)shape.ActiveXControl;

            list.ListFillRange = ("A3:A7");
            list.Value = ("Apple");
            list.LinkedCell = ("A1");
            list.ListStyle = (ControlListStyle.Option);
            list.SelectionType = (SelectionType.Multi);

            // Anzeigen der anfänglichen Data-Eigenschaftsinformationen
            Console.WriteLine("Initial Data length: " + list.Data.Length);

            // Steuerelementeigenschaften ändern, die Data beeinflussen
            list.BackOleColor = 0xFF0000;

            // Aktualisierte Data-Eigenschaftsinformationen anzeigen
            Console.WriteLine("Modified Data length: " + list.Data.Length);

            // Speichere die Arbeitsmappe, um persistente Änderungen zu demonstrieren
            workbook.Save("ActiveXControlDataDemo.xlsx");

        }
    }
}
```

### Siehe auch

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


