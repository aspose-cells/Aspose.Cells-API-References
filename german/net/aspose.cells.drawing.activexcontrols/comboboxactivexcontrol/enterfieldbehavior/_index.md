---
title: "ComboBoxActiveXControl.EnterFieldBehavior"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl property. Gibt das Auswahlverhalten beim Betreten des Steuerelements an. True gibt an, dass die Auswahl unverändert bleibt seit dem letzten Mal, als das Steuerelement aktiv war. False gibt an, dass beim Betreten des Steuerelements der gesamte Text im Steuerelement ausgewählt wird."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/enterfieldbehavior/
---
## ComboBoxActiveXControl.EnterFieldBehavior property

Gibt das Auswahlverhalten beim Betreten des Steuerelements an. True gibt an, dass die Auswahl unverändert bleibt seit dem letzten Mal, als das Steuerelement aktiv war. False gibt an, dass beim Betreten des Steuerelements der gesamte Text im Steuerelement ausgewählt wird.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erste ComboBox ActiveX-Steuerung hinzufügen
            Shape shape1 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 50
            );
            ComboBoxActiveXControl combo1 = (ComboBoxActiveXControl)shape1.ActiveXControl;
            combo1.EnterFieldBehavior = false; // Default behavior (select all text on entry)
            combo1.Value = "Select Option";
            combo1.BorderStyle = ControlBorderType.Single;
            
            // Zweite ComboBox ActiveX-Steuerung hinzufügen
            Shape shape2 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 2, 0, 100, 50
            );
            ComboBoxActiveXControl combo2 = (ComboBoxActiveXControl)shape2.ActiveXControl;
            combo2.EnterFieldBehavior = true; // Preserve previous selection
            combo2.Value = "Edit Value";
            combo2.BorderStyle = ControlBorderType.Single;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxActiveXControlDemo.xlsm", SaveFormat.Xlsm);
            
            // Eigenschaftseinstellungen überprüfen
            Console.WriteLine("Combo1 EnterFieldBehavior: " + combo1.EnterFieldBehavior);
            Console.WriteLine("Combo2 EnterFieldBehavior: " + combo2.EnterFieldBehavior);
        }
    }
}
```

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


