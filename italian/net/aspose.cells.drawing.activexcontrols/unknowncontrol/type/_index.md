---
title: "UnknownControl.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnknownControl. Ottiene il tipo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/unknowncontrol/type/
---
## UnknownControl.Type property

Ottiene il tipo del controllo ActiveX.

```csharp
public override ControlType Type { get; }
```

### Esempi

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
            // Carica la cartella di lavoro esistente contenente il controllo sconosciuto
            Workbook workbook = new Workbook("input_with_unknown_control.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            // Trova e elabora le istanze di UnknownControl
            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.ActiveXControl is UnknownControl control)
                {
                    // Dimostra la lettura della proprietà Type
                    Console.WriteLine($"Found control with Type: {control.Type}");
                    
                    // Esempio di utilizzo basato sul tipo di controllo
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

            // Salva la cartella di lavoro elaborata
            workbook.Save("ControlTypeAnalysis.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlType](../../controltype/)
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


