---
title: "ComboBoxActiveXControl.MatchEntry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl-Eigenschaft. Gibt an, wie eine ListBox oder ein ComboBox ihre Liste durchsucht, während der Benutzer tippt"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/matchentry/
---
## ComboBoxActiveXControl.MatchEntry property

Gibt an, wie eine ListBox oder ComboBox ihre Liste durchsucht, während der Benutzer tippt.

```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein ComboBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 20);
            
            // Abrufen des ComboBox ActiveX-Steuerelements
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Grundlegende Eigenschaften konfigurieren
            comboBox.Font.Name = "Arial";
            comboBox.Font.Size = 10;
            comboBox.ListRows = 8;

            // Demonstrieren Sie die MatchEntry-Eigenschaft
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Search as user types
            Console.WriteLine("MatchEntry set to: " + comboBox.MatchEntry);

            // Ändern Sie MatchEntry in einen anderen Modus
            comboBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Search by first letter
            Console.WriteLine("MatchEntry changed to: " + comboBox.MatchEntry);

            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxActiveXControlDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


