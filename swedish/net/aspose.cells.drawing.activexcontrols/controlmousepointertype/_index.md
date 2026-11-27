---
title: "Enum ControlMousePointerType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType enum. Representerar typen av ikon som visas som muspekare för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlmousepointertype/
---
## ControlMousePointerType enumeration

Representerar ikontypen som visas som muspekaren för kontrollen.

```csharp
public enum ControlMousePointerType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Standardpekare. |
| Arrow | `1` | Pil. |
| Cross | `2` | Korshårspenna. |
| IBeam | `3` | I-balk. |
| SizeNESW | `6` | Dubbelpil som pekar åt nordost och sydväst. |
| SizeNS | `7` | Dubbelpil som pekar åt norr och söder. |
| SizeNWSE | `8` | Dubbelpil som pekar åt nordväst och sydost. |
| SizeWE | `9` | Dubbelpil som pekar åt väst och öst. |
| UpArrow | `10` | Uppåtpil. |
| HourGlass | `11` | Timglas. |
| NoDrop | `12` | "Not"-symbol (cirkel med en diagonal linje) ovanpå objektet som dras. |
| AppStarting | `13` | Pil med ett timglas. |
| Help | `14` | Pil med ett frågetecken. |
| SizeAll | `15` | "Size-all"-pekare (pilar som pekar åt norr, söder, öster och väster). |
| Custom | `99` | Använder ikonen som anges av egenskapen MouseIcon. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlMousePointerTypeDemo
    {
        public static void ControlMousePointerTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ActiveX-kontroll på kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Kasta ActiveXControl till ActiveXControlBase för att komma åt dess egenskaper
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // Ställ in muspekartypen för kontrollen
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // Ställ in andra egenskaper för demonstration
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // Spara arbetsboken
            workbook.Save("ControlMousePointerTypeExample.xlsx");
            workbook.Save("ControlMousePointerTypeExample.pdf");

            // Skriv ut resultatet
            Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


