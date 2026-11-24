---
title: "Aufzählung ControlMatchEntryType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType Aufzählung. Stellt dar, wie eine ListBox oder ComboBox ihre Liste durchsucht, während der Benutzer tippt"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enumeration

Stellt dar, wie eine ListBox oder ComboBox ihre Liste durchsucht, während der Benutzer tippt.

```csharp
public enum ControlMatchEntryType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| FirstLetter | `0` | Das Steuerelement sucht nach dem nächsten Eintrag, der mit dem eingegebenen Zeichen beginnt. Durch wiederholtes Drücken desselben Buchstabens werden alle Einträge, die mit diesem Buchstaben beginnen, durchlaufen. |
| Complete | `1` | Während jedes Zeichen eingegeben wird, sucht das Steuerelement nach einem Eintrag, der allen eingegebenen Zeichen entspricht. |
| None | `2` | Die Liste wird nicht durchsucht, wenn Zeichen eingegeben werden. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Füge ein ComboBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Setze Eigenschaften für die ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // Fügen Sie Elemente zur ComboBox hinzu
            comboBox.Value = "Apple;Banana;Cherry";

            // Fügen Sie ein ListBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Legen Sie Eigenschaften für die ListBox fest
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // Elemente zur ListBox hinzufügen
            listBox.Value = "Apple;Banana;Cherry";

            // Speichere die Arbeitsmappe
            workbook.Save("ControlMatchEntryTypeExample.xlsx");
            workbook.Save("ControlMatchEntryTypeExample.pdf");

            // Ergebnisse ausgeben
            Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


