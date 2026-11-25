---
title: "ActiveXControlBase.ForeOleColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ActiveXControlBase proprietà. Ottiene e imposta il colore ole del primo piano"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/
---
## ActiveXControlBase.ForeOleColor property

Ottiene e imposta il colore OLE del primo piano.

```csharp
public virtual int ForeOleColor { get; set; }
```

### Osservazioni

Non si applica al controllo Image.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyForeOleColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo CheckBox ActiveX con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà di base
            checkBox.Caption = "Sample CheckBox";
            checkBox.IsAutoSize = true;

            // Dimostrare la proprietà ForeOleColor
            checkBox.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            checkBox.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);

            // Salva la cartella di lavoro
            workbook.Save("ActiveXControlForeOleColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


