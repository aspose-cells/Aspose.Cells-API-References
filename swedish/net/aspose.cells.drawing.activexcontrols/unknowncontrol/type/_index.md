---
title: "UnknownControl.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnknownControl egenskap. Hämtar typen av ActiveX-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/unknowncontrol/type/
---
## UnknownControl.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public override ControlType Type { get; }
```

### Exempel

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
            // Läs in befintlig arbetsbok som innehåller okänd kontroll
            Workbook workbook = new Workbook("input_with_unknown_control.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            // Hitta och bearbeta UnknownControl-instanser
            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.ActiveXControl is UnknownControl control)
                {
                    // Demonstrera läsning av Type-egenskapen
                    Console.WriteLine($"Found control with Type: {control.Type}");
                    
                    // Exempel på användning baserat på kontrolltyp
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

            // Spara bearbetad arbetsbok
            workbook.Save("ControlTypeAnalysis.xlsx");
        }
    }
}
```

### Se även

* enum [ControlType](../../controltype/)
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


