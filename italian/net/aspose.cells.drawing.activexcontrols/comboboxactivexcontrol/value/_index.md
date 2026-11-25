---
title: "ComboBoxActiveXControl.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBoxActiveXControl. Ottiene e imposta il valore del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/value/
---
## ComboBoxActiveXControl.Value property

Ottiene e imposta il valore del controllo.

```csharp
public string Value { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ComboBox al foglio di lavoro
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 1, 0, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il ComboBox
            comboBox.Value = "Initial Value";
            comboBox.ListFillRange = "A1:A3";
            
            // Aggiungi alcuni dati di esempio all'intervallo dell'elenco
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Aggiorna il valore selezionato dalla cella collegata
            worksheet.Cells["B1"].PutValue("Option 2");
            worksheet.Shapes.UpdateSelectedValue();

            // Dimostra come ottenere la proprietà Value
            Console.WriteLine("ComboBox Value: " + comboBox.Value);

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


