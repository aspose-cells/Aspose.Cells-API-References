---
title: "Enum DropButtonStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle enum. Representerar symbolen som visas på rullknappen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/dropbuttonstyle/
---
## DropButtonStyle enumeration

Representerar symbolen som visas på drop button.

```csharp
public enum DropButtonStyle
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Plain | `0` | Visar en knapp utan symbol. |
| Arrow | `1` | Visar en knapp med en nedåtpil. |
| Ellipsis | `2` | Visar en knapp med en ellips (...). |
| Reduce | `3` | Visar en knapp med ett horisontellt streck som ett understreckstecken. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class DropButtonStyleDemo
    {
        public static void DropButtonStyleExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow

            // Lägg till några objekt i ComboBoxen
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            comboBox.ListFillRange = "A1:A4";

            // Spara arbetsboken
            workbook.Save("DropButtonStyleExample.xlsx");
            workbook.Save("DropButtonStyleExample.pdf");

            // Skriv ut den använda DropButtonStyle
            Console.WriteLine("DropButtonStyle set to: " + comboBox.DropButtonStyle);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


