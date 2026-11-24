---
title: "StyleFlag.Rotation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Drehungs-Einstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

Die Rotationseinstellung wird angewendet.

```csharp
public bool Rotation { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf Zelle A1 zu und setze etwas Text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // Ermitteln Sie den Stil der Zelle
            Style style = workbook.CreateStyle();

            // Setze neuen Drehwert (45 Grad)
            style.RotationAngle = 45;

            // Zeige aktuellen Drehwert an
            Console.WriteLine("Current Rotation value: " + cell.GetStyle().RotationAngle);            

            // Erstelle ein StyleFlag und aktiviere das Drehungs-Flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // Wende den Stil mit Drehung auf die Zelle an
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("after setting style, rotation value: " + cell.GetStyle().RotationAngle);
           
            // Ergebnis speichern
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


