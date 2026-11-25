---
title: "ComboBoxActiveXControl.BorderOleColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBoxActiveXControl. Ottiene e imposta il colore ole dello sfondo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderolecolor/
---
## ComboBoxActiveXControl.BorderOleColor property

Ottiene e imposta il colore ole dello sfondo.

```csharp
public int BorderOleColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ComboBox al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                1, 1, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà di base
            comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Dimostra la proprietà BorderOleColor
            comboBox.BorderOleColor = ColorTranslator.ToOle(Color.Red); // Set border color to red
            
            // Imposta del testo di esempio
            comboBox.Value = "Border Color Demo";

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxBorderColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


