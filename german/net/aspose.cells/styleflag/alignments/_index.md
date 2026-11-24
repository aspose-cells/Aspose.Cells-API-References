---
title: "StyleFlag.Alignments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Ausrichtungseinstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/alignments/
---
## StyleFlag.Alignments property

Ausrichtungseinstellung wird angewendet.

```csharp
public bool Alignments { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyAlignmentsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf Zelle A1 zu und setze etwas Text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Erstellen Sie ein Style-Objekt und setzen Sie die Ausrichtungseigenschaften
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.RotationAngle = 45;

            // Erstellen Sie ein Style-Flag und aktivieren Sie die Ausrichtungseigenschaften
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Alignments = true;

            // Den Stil mit dem StyleFlag auf die Zelle anwenden
            cell.SetStyle(style, styleFlag);

            // Zeigen Sie die aktuellen Ausrichtungseinstellungen an
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Ändern Sie das Style-Flag, um die Ausrichtungseigenschaften zu deaktivieren
            styleFlag.Alignments = false;
            
            // Erstellen Sie einen neuen Stil mit anderer Ausrichtung
            Style newStyle = workbook.CreateStyle();
            newStyle.HorizontalAlignment = TextAlignmentType.Right;
            newStyle.VerticalAlignment = TextAlignmentType.Top;
            newStyle.RotationAngle = 0;

            // Wenden Sie den neuen Stil an – die Ausrichtungen ändern sich nicht, weil das Flag false ist
            cell.SetStyle(newStyle, styleFlag);

            // Zeigen Sie die unveränderten Ausrichtungseinstellungen an
            Console.WriteLine("After applying new style with Alignments=false:");
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Speichere die Arbeitsmappe
            workbook.Save("StyleFlagAlignmentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


