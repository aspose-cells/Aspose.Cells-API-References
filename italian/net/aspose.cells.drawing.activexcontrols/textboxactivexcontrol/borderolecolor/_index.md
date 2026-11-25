---
title: "TextBoxActiveXControl.BorderOleColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Ottiene e imposta il colore OLE dello sfondo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderolecolor/
---
## TextBoxActiveXControl.BorderOleColor property

Ottiene e imposta il colore ole dello sfondo.

```csharp
public int BorderOleColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox e ottieni la sua proprietà ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 100, 100, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà BorderOleColor (sistema di colore predefinito di Excel 12 o verde)
            textBox.BorderOleColor = unchecked((int)0x80000012);

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlBorderOleColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


