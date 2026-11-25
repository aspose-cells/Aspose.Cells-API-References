---
title: "ComboBoxActiveXControl.EnterFieldBehavior"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ComboBoxActiveXControl property. Specifica il comportamento di selezione quando si entra nel controllo. True specifica che la selezione rimane invariata rispetto all'ultima volta che il controllo era attivo. False specifica che tutto il testo nel controllo verrà selezionato quando si entra nel controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/enterfieldbehavior/
---
## ComboBoxActiveXControl.EnterFieldBehavior property

Specifica il comportamento di selezione quando si entra nel controllo. True indica che la selezione rimane invariata rispetto all'ultima volta che il controllo era attivo. False indica che tutto il testo nel controllo verrà selezionato all'ingresso.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi il primo controllo ComboBox ActiveX
            Shape shape1 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 50
            );
            ComboBoxActiveXControl combo1 = (ComboBoxActiveXControl)shape1.ActiveXControl;
            combo1.EnterFieldBehavior = false; // Default behavior (select all text on entry)
            combo1.Value = "Select Option";
            combo1.BorderStyle = ControlBorderType.Single;
            
            // Aggiungi il secondo controllo ComboBox ActiveX
            Shape shape2 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 2, 0, 100, 50
            );
            ComboBoxActiveXControl combo2 = (ComboBoxActiveXControl)shape2.ActiveXControl;
            combo2.EnterFieldBehavior = true; // Preserve previous selection
            combo2.Value = "Edit Value";
            combo2.BorderStyle = ControlBorderType.Single;
            
            // Salva la cartella di lavoro
            workbook.Save("ComboBoxActiveXControlDemo.xlsm", SaveFormat.Xlsm);
            
            // Verifica le impostazioni della proprietà
            Console.WriteLine("Combo1 EnterFieldBehavior: " + combo1.EnterFieldBehavior);
            Console.WriteLine("Combo2 EnterFieldBehavior: " + combo2.EnterFieldBehavior);
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


