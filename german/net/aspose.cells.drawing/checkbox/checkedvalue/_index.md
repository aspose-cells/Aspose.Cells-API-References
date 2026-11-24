---
title: "CheckBox.CheckedValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBox-Eigenschaft. Gibt den Wert des Kontrollkästchens zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

Liest oder setzt den Wert des Kontrollkästchens.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyCheckedValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie ein Kontrollkästchen zum Arbeitsblatt hinzu
            CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);

            // Setzen Sie den Wert des Kontrollkästchens auf Aktiviert
            checkBox.CheckedValue = CheckValueType.Checked;

            // Speichere die Arbeitsmappe
            workbook.Save("CheckBoxCheckedValueDemo.xlsx");

            // Lade die gespeicherte Arbeitsmappe zum Überprüfen
            Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
            CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Geben Sie den Zustand des Kontrollkästchens aus
            Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
        }
    }
}
```

### Siehe auch

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


