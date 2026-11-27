---
title: "ActiveXControlBase.Data"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar och anger den binära datan för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/data/
---
## ActiveXControlBase.Data property

Hämtar och anger den binära datan för kontrollen.

```csharp
public virtual byte[] Data { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
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

            // Visa information om den initiala Data-egenskapen
            Console.WriteLine("Initial Data length: " + list.Data.Length);

            // Ändra kontrollens egenskaper som påverkar Data
            list.BackOleColor = 0xFF0000;

            // Visa uppdaterad information om Data-egenskapen
            Console.WriteLine("Modified Data length: " + list.Data.Length);

            // Spara arbetsboken för att demonstrera bestående ändringar
            workbook.Save("ActiveXControlDataDemo.xlsx");

        }
    }
}
```

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


