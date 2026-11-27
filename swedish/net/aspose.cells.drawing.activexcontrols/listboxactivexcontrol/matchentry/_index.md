---
title: "ListBoxActiveXControl.MatchEntry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Anger hur en ListBox eller ComboBox söker i sin lista när användaren skriver"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/matchentry/
---
## ListBoxActiveXControl.MatchEntry property

Indikerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver.

```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyMatchEntryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");

            // Lägg till ListBox ActiveX‑kontroll
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 1, 0, 100, 80);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera ListBox‑egenskaper
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.Value = "Apple;Banana;Cherry;Date";

            // Spara arbetsboken
            workbook.Save("ListBoxMatchEntryDemo.xlsx");

            Console.WriteLine("ListBox with FirstLetter MatchEntry created successfully.");
        }
    }
}
```

### Se även

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


