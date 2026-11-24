---
title: "ComboBoxActiveXControl.IsAutoWordSelected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl-Eigenschaft. Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. True gibt an, dass die Basiseinheit ein einzelnes Zeichen ist. false gibt an, dass die Basiseinheit ein ganzes Wort ist."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isautowordselected/
---
## ComboBoxActiveXControl.IsAutoWordSelected property

Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. True gibt an, dass die Basiseinheit ein einzelnes Zeichen ist. false gibt an, dass die Basiseinheit ein ganzes Wort ist.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein ComboBox ActiveX-Steuerelement mit allen erforderlichen Parametern hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 100, 20, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Grundlegende Eigenschaften konfigurieren
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.Value = "Sample Text";

            // IsAutoWordSelected-Eigenschaft demonstrieren
            comboBox.IsAutoWordSelected = false;
            Console.WriteLine("IsAutoWordSelected set to: " + comboBox.IsAutoWordSelected);

            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxIsAutoWordSelectedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


