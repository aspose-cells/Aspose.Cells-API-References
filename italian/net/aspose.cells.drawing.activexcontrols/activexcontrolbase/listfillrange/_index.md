---
title: "ActiveXControlBase.ListFillRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControlBase. Ottiene e imposta l'intervallo di riempimento della lista"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/
---
## ActiveXControlBase.ListFillRange property

Ottiene e imposta l'intervallo di riempimento dell'elenco.

```csharp
public string ListFillRange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyListFillRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per ListFillRange
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
            }

            // Aggiungi un ComboBoxActiveXControl
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1, 0, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta ListFillRange per popolare la casella combinata
            comboBox.ListFillRange = "A2:A10";

            // Salva la cartella di lavoro
            workbook.Save("ActiveXControlListFillRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


