---
title: "CellsHelper.GetUsedColors"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt alle im Arbeitsbuch verwendeten Farben zurück"
type: docs
url: /de/net/aspose.cells/cellshelper/getusedcolors/
---
## CellsHelper.GetUsedColors method

Ermittelt alle im Arbeitsbuch verwendeten Farben.

```csharp
public static Color[] GetUsedColors(Workbook workbook)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Arbeitsmappe | Arbeitsmappe | Das Arbeitsmappen-Objekt. |

### Rückgabewert

Die verwendeten Farben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsHelperMethodGetUsedColorsWithWorkbookDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige farbige Zellen hinzu, um die verwendeten Farben zu demonstrieren
            worksheet.Cells["A1"].PutValue("Red Cell");
            worksheet.Cells["A1"].GetStyle().ForegroundColor = Color.Red;
            worksheet.Cells["A1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["A1"].SetStyle(worksheet.Cells["A1"].GetStyle());

            worksheet.Cells["B1"].PutValue("Blue Cell");
            worksheet.Cells["B1"].GetStyle().ForegroundColor = Color.Blue;
            worksheet.Cells["B1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["B1"].SetStyle(worksheet.Cells["B1"].GetStyle());

            worksheet.Cells["C1"].PutValue("Green Cell");
            worksheet.Cells["C1"].GetStyle().ForegroundColor = Color.Green;
            worksheet.Cells["C1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["C1"].SetStyle(worksheet.Cells["C1"].GetStyle());

            try
            {
                // Rufen Sie die Methode GetUsedColors mit dem Parameter workbook auf
                Color[] usedColors = CellsHelper.GetUsedColors(workbook);

                // Zeigen Sie die verwendeten Farben an
                Console.WriteLine("Used colors in the workbook:");
                foreach (Color color in usedColors)
                {
                    Console.WriteLine($"Color: A={color.A}, R={color.R}, G={color.G}, B={color.B}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetUsedColors method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CellsHelperGetUsedColorsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../../workbook/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


