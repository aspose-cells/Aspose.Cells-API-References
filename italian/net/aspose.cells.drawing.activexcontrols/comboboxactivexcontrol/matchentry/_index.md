---
title: "ComboBoxActiveXControl.MatchEntry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBoxActiveXControl. Indica come un ListBox o ComboBox ricerca la sua lista mentre l'utente digita"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/matchentry/
---
## ComboBoxActiveXControl.MatchEntry property

Indica come un ListBox o ComboBox ricerca l'elenco mentre l'utente digita.

```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyMatchEntryDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ComboBox al foglio di lavoro
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 20);
            
            // Ottieni il controllo ComboBox ActiveX
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà di base
            comboBox.Font.Name = "Arial";
            comboBox.Font.Size = 10;
            comboBox.ListRows = 8;

            // Dimostra la proprietà MatchEntry
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Search as user types
            Console.WriteLine("MatchEntry set to: " + comboBox.MatchEntry);

            // Cambia MatchEntry in un'altra modalità
            comboBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Search by first letter
            Console.WriteLine("MatchEntry changed to: " + comboBox.MatchEntry);

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxActiveXControlDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


