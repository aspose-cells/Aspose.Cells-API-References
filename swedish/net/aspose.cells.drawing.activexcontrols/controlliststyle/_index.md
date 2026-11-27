---
title: "Enum ControlListStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlListStyle enum. Representerar det visuella utseendet på listan i en ListBox eller ComboBox"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlliststyle/
---
## ControlListStyle enumeration

Representerar det visuella utseendet på listan i en ListBox eller ComboBox.

```csharp
public enum ControlListStyle
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Plain | `0` | Visar en lista där bakgrunden på ett objekt markeras när det är valt. |
| Option | `1` | Visar en lista där en alternativknapp eller en kryssruta bredvid varje post visar urvalstillståndet för det objektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlListStyleDemo
    {
        public static void ControlListStyleExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");

            // Lägg till en ComboBox ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.ListStyle = ControlListStyle.Plain; // Set the ListStyle to Plain

            // Lägg till objekt i ComboBoxen
            comboBox.Value = "Item 1";
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;

            // Lägg till en ListBox ActiveX‑kontroll i kalkylbladet
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Ställ in egenskaper för ListBoxen
            listBox.ColumnCount = 1;
            listBox.ListStyle = ControlListStyle.Option; // Set the ListStyle to Option

            // Lägg till objekt i ListBoxen
            listBox.Value = "Item 1";
            listBox.BoundColumn = 1;
            listBox.TextColumn = 1;

            // Spara arbetsboken
            workbook.Save("ControlListStyleExample.xlsx");
            workbook.Save("ControlListStyleExample.pdf");

            // Skriv ut resultaten
            Console.WriteLine("ComboBox ListStyle: " + comboBox.ListStyle);
            Console.WriteLine("ListBox ListStyle: " + listBox.ListStyle);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


