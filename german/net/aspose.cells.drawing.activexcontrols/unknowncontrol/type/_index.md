---
title: "UnknownControl.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnknownControl-Eigenschaft. Ruft den Typ des ActiveX-Steuerelements ab"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/unknowncontrol/type/
---
## UnknownControl.Type property

Liest den Typ des ActiveX-Steuerelements.

```csharp
public override ControlType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Lade vorhandene Arbeitsmappe, die ein unbekanntes Steuerelement enthält
            Workbook workbook = new Workbook("input_with_unknown_control.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            // Finde und verarbeite UnknownControl-Instanzen
            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.ActiveXControl is UnknownControl control)
                {
                    // Demonstriere das Auslesen der Type-Eigenschaft
                    Console.WriteLine($"Found control with Type: {control.Type}");
                    
                    // Beispielhafte Verwendung basierend auf dem Steuertyp
                    if (control.Type == ControlType.ListBox)
                    {
                        Console.WriteLine("Processing legacy ListBox control");
                    }
                    else if (control.Type == ControlType.Unknown)
                    {
                        Console.WriteLine("Handling completely unknown control type");
                    }
                }
            }

            // Speichere verarbeitete Arbeitsmappe
            workbook.Save("ControlTypeAnalysis.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlType](../../controltype/)
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


