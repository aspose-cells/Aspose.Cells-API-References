---
title: "TextBoxActiveXControl.IsAutoTab"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se il focus si sposterà automaticamente al controllo successivo quando l'utente inserisce il numero massimo di caratteri"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab/
---
## TextBoxActiveXControl.IsAutoTab property

Indica se il focus si sposterà automaticamente al controllo successivo quando l'utente inserisce il numero massimo di caratteri.

```csharp
public bool IsAutoTab { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoTabDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo TextBox ActiveX e ottieni il suo controllo
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 30, 100, 30);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà IsAutoTab
            Console.WriteLine("Initial IsAutoTab value: " + textBoxControl.IsAutoTab);
            
            // Imposta IsAutoTab su true se è false
            if (!textBoxControl.IsAutoTab)
            {
                textBoxControl.IsAutoTab = true;
                Console.WriteLine("IsAutoTab set to: " + textBoxControl.IsAutoTab);
            }

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlIsAutoTabDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


