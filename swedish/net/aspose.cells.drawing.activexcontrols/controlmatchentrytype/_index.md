---
title: "Enum ControlMatchEntryType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType-enum. Representerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enumeration

Representerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver.

```csharp
public enum ControlMatchEntryType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| FirstLetter | `0` | Kontrollen söker efter nästa post som börjar med det angivna tecknet. Att upprepade gånger skriva samma bokstav cyklar igenom alla poster som börjar med den bokstaven. |
| Complete | `1` | När varje tecken skrivs in söker kontrollen efter en post som matchar alla angivna tecken. |
| None | `2` | Listan kommer inte att sökas när tecken skrivs in. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Lägg till en ComboBox ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // Lägg till objekt i ComboBoxen
            comboBox.Value = "Apple;Banana;Cherry";

            // Lägg till en ListBox ActiveX‑kontroll i kalkylbladet
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Ställ in egenskaper för ListBoxen
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // Lägg till objekt i ListBoxen
            listBox.Value = "Apple;Banana;Cherry";

            // Spara arbetsboken
            workbook.Save("ControlMatchEntryTypeExample.xlsx");
            workbook.Save("ControlMatchEntryTypeExample.pdf");

            // Skriv ut resultaten
            Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


