---
title: "Enum ControlMousePointerType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType-Enum. Stellt den Typ des als Mauszeiger für das Steuerelement angezeigten Symbols dar"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlmousepointertype/
---
## ControlMousePointerType enumeration

Stellt den Typ des als Mauszeiger angezeigten Symbols für das Steuerelement dar.

```csharp
public enum ControlMousePointerType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Standardzeiger. |
| Arrow | `1` | Pfeil. |
| Cross | `2` | Fadenkreuzzeiger. |
| IBeam | `3` | I‑Strich. |
| SizeNESW | `6` | Doppelter Pfeil, der nach Nordost und Südwest zeigt. |
| SizeNS | `7` | Doppelter Pfeil, der nach Norden und Süden zeigt. |
| SizeNWSE | `8` | Doppelter Pfeil, der nach Nordwesten und Südosten zeigt. |
| SizeWE | `9` | Doppelter Pfeil, der nach Westen und Osten zeigt. |
| UpArrow | `10` | Pfeil nach oben. |
| HourGlass | `11` | Sanduhr. |
| NoDrop | `12` | "Nicht"-Symbol (Kreis mit einem diagonalen Strich) über dem zu ziehenden Objekt. |
| AppStarting | `13` | Pfeil mit einer Sanduhr. |
| Help | `14` | Pfeil mit einem Fragezeichen. |
| SizeAll | `15` | "Size-all"-Cursor (Pfeile, die nach Norden, Süden, Osten und Westen zeigen). |
| Custom | `99` | Verwendet das Symbol, das durch die Eigenschaft MouseIcon angegeben ist. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Wandeln Sie das ActiveXControl in ActiveXControlBase um, um auf dessen Eigenschaften zuzugreifen
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // Legen Sie den Mauszeigertyp für das Steuerelement fest
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // Legen Sie weitere Eigenschaften zur Demonstration fest
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ControlMousePointerTypeExample.xlsx");
            workbook.Save("ControlMousePointerTypeExample.pdf");

            // Gib das Ergebnis aus
            Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


