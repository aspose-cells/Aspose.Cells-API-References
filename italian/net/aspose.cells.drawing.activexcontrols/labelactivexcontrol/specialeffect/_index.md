---
title: "LabelActiveXControl.SpecialEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LabelActiveXControl proprietà. Ottiene e imposta l'effetto speciale del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/specialeffect/
---
## LabelActiveXControl.SpecialEffect property

Ottiene e imposta l'effetto speciale del controllo.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un Label ActiveX Control con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 100, 50,  // upperLeftRow, upperLeftColumn, height, width
                100, 50);       // heightInPx, widthInPx
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà di base
            labelControl.Caption = "Sample Label";
            labelControl.IsWordWrapped = true;

            // Dimostrare la proprietà SpecialEffect
            labelControl.SpecialEffect = ControlSpecialEffectType.Raised;
            Console.WriteLine("SpecialEffect set to: " + labelControl.SpecialEffect);

            // Modifica SpecialEffect e mostra la differenza
            labelControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            Console.WriteLine("SpecialEffect changed to: " + labelControl.SpecialEffect);

            // Salva la cartella di lavoro
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


