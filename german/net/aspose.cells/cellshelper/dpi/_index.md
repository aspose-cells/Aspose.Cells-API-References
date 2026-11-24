---
title: "CellsHelper.DPI"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Eigenschaft. Gibt die DPI des Geräts zurück"
type: docs
url: /de/net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

Liest die DPI des Geräts.

```csharp
public static double DPI { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyDPIDemo
    {
        public static void Run()
        {
            // Aktuelle DPI festlegen und anzeigen
            Console.WriteLine("Original DPI: " + CellsHelper.DPI);
            
            // DPI-Einstellung ändern
            CellsHelper.DPI = 300;
            Console.WriteLine("New DPI: " + CellsHelper.DPI);

            // Erstelle eine neue Arbeitsmappe und speichere sie mit unterschiedlichen DPI-Einstellungen
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge ein Beispiel-Shape hinzu, um die DPI-Auswirkung zu demonstrieren
            sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);

            // Mit aktueller DPI-Einstellung speichern
            workbook.Save("output_with_dpi_300.xlsx");

            // DPI ändern und erneut speichern
            CellsHelper.DPI = 96;
            workbook.Save("output_with_dpi_96.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


