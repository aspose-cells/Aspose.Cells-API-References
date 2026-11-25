---
title: "ActiveXControl.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControl. Rappresenta il font del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrol/font/
---
## ActiveXControl.Font property

Rappresenta il font del controllo.

```csharp
public Font Font { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlPropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi un controllo ActiveX (Label) al foglio di lavoro
                Shape shape = worksheet.Shapes.AddActiveXControl(
                    ControlType.Label,
                    1, 1, 200, 50,
                    0, 0);

                // Ottieni l'istanza del controllo ActiveX
                LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

                // Imposta alcune proprietà di base
                label.Caption = "Sample Label";

                // Accedi alla proprietà Font (sola lettura)
                Font controlFont = label.Font;

                // Visualizza le proprietà del font
                Console.WriteLine("Font Name: " + controlFont.Name);
                Console.WriteLine("Font Size: " + controlFont.Size);
                Console.WriteLine("Is Bold: " + controlFont.IsBold);
                Console.WriteLine("Is Italic: " + controlFont.IsItalic);
                Console.WriteLine("Color: " + controlFont.Color);
                Console.WriteLine("Underline Type: " + controlFont.Underline);

                // Salva la cartella di lavoro
                workbook.Save("FontDemo.xlsx");
                Console.WriteLine("Font properties demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


