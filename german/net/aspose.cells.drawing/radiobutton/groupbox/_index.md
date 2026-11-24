---
title: "RadioButton.GroupBox"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RadioButton-Eigenschaft. Gibt die GroupBox zurück, die diesen RadioButton enthält"
type: docs
url: /de/net/aspose.cells.drawing/radiobutton/groupbox/
---
## RadioButton.GroupBox property

Liest die GroupBox, die diesen RadioButton enthält.

```csharp
public GroupBox GroupBox { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonPropertyGroupBoxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine GroupBox hinzu, die RadioButtons enthält
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);
            groupBox.Name = "OptionsGroup";
            groupBox.Shadow = true;

            // Füge RadioButtons zum Arbeitsblatt hinzu (noch nicht in der GroupBox)
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);

            // Anfangswerte der GroupBox-Eigenschaften anzeigen (sollte null sein)
            Console.WriteLine("RadioButton1 GroupBox before grouping: " + (radioButton1.GroupBox == null ? "null" : radioButton1.GroupBox.Name));
            Console.WriteLine("RadioButton2 GroupBox before grouping: " + (radioButton2.GroupBox == null ? "null" : radioButton2.GroupBox.Name));

            // Füge RadioButtons zur GroupBox hinzu, indem du die Platzierung festlegst
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;

            // Verschiebe RadioButtons innerhalb der GroupBox
            radioButton1.Top = groupBox.Top + 20;
            radioButton1.Left = groupBox.Left + 20;
            radioButton2.Top = groupBox.Top + 50;
            radioButton2.Left = groupBox.Left + 20;

            // GroupBox-Eigenschaftswerte nach dem Gruppieren anzeigen
            Console.WriteLine("RadioButton1 GroupBox after grouping: " + radioButton1.GroupBox.Name);
            Console.WriteLine("RadioButton2 GroupBox after grouping: " + radioButton2.GroupBox.Name);

            // Gruppenverhalten demonstrieren
            radioButton1.IsChecked = true;
            Console.WriteLine("RadioButton1 checked state: " + radioButton1.IsChecked);
            Console.WriteLine("RadioButton2 checked state: " + radioButton2.IsChecked);

            // Ergebnis speichern
            workbook.Save("RadioButtonPropertyGroupBoxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GroupBox](../../groupbox/)
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


