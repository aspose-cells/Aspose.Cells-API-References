---
title: "ComboBoxActiveXControl.IsAutoWordSelected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBoxActiveXControl. Specifica l'unità di base usata per estendere una selezione. True indica che l'unità di base è un singolo carattere. false indica che l'unità di base è una parola intera"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isautowordselected/
---
## ComboBoxActiveXControl.IsAutoWordSelected property

Specifica l'unità di base utilizzata per estendere una selezione. True specifica che l'unità di base è un singolo carattere. false specifica che l'unità di base è una parola intera.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ComboBox ActiveX con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 100, 20, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà di base
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.Value = "Sample Text";

            // Dimostra la proprietà IsAutoWordSelected
            comboBox.IsAutoWordSelected = false;
            Console.WriteLine("IsAutoWordSelected set to: " + comboBox.IsAutoWordSelected);

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxIsAutoWordSelectedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


