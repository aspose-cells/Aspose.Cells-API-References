---
title: "ComboBoxActiveXControl.MatchEntry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Anger hur en ListBox eller ComboBox söker i sin lista när användaren skriver"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/matchentry/
---
## ComboBoxActiveXControl.MatchEntry property

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
    public class ComboBoxActiveXControlPropertyMatchEntryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll i kalkylbladet
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 20);
            
            // Hämta ComboBox ActiveX-kontrollen
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera grundläggande egenskaper
            comboBox.Font.Name = "Arial";
            comboBox.Font.Size = 10;
            comboBox.ListRows = 8;

            // Demonstrera egenskapen MatchEntry
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Search as user types
            Console.WriteLine("MatchEntry set to: " + comboBox.MatchEntry);

            // Ändra MatchEntry till ett annat läge
            comboBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Search by first letter
            Console.WriteLine("MatchEntry changed to: " + comboBox.MatchEntry);

            // Spara arbetsboken
            workbook.Save("ComboBoxActiveXControlDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


