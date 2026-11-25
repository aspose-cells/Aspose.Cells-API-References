---
title: "Enum ControlMatchEntryType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType. Rappresenta come un ListBox o ComboBox ricerca la sua lista mentre l'utente digita"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enumeration

Rappresenta come una ListBox o ComboBox ricerca l'elenco mentre l'utente digita.

```csharp
public enum ControlMatchEntryType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| FirstLetter | `0` | Il controllo ricerca la voce successiva che inizia con il carattere inserito. Digitare ripetutamente la stessa lettera scorre tutte le voci che iniziano con quella lettera. |
| Complete | `1` | Man mano che ogni carattere viene digitato, il controllo cerca una voce che corrisponda a tutti i caratteri inseriti. |
| None | `2` | L'elenco non verrà cercato quando vengono digitati i caratteri. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ControlMatchEntryTypeDemo
    {
        public static void ControlMatchEntryTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Aggiungi un controllo ActiveX ComboBox al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // Aggiungi elementi al ComboBox
            comboBox.Value = "Apple;Banana;Cherry";

            // Aggiungi un controllo ActiveX ListBox al foglio di lavoro
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Imposta le proprietà per il ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // Aggiungi elementi al ListBox
            listBox.Value = "Apple;Banana;Cherry";

            // Salva la cartella di lavoro
            workbook.Save("ControlMatchEntryTypeExample.xlsx");
            workbook.Save("ControlMatchEntryTypeExample.pdf");

            // Restituisci i risultati
            Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


