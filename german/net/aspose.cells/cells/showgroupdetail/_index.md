---
title: "Cells.ShowGroupDetail"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Erweitert die gruppierten Zeilen/Spalten"
type: docs
url: /de/net/aspose.cells/cells/showgroupdetail/
---
## Cells.ShowGroupDetail method

Erweitert die gruppierten Zeilen/Spalten.

```csharp
public void ShowGroupDetail(bool isVertical, int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isVertical | Boolean | Wahr, erweitert die gruppierten Zeilen. |
| Index | Int32 | Der Zeilen-/Spaltenindex |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodShowGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten in den Zeilen 5‑7 einfügen (nullbasierter Index 4‑6)
            for (int row = 4; row <= 6; row++)
            {
                worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
            }

            // Gruppiere Zeilen 4‑6 (Excel‑Zeilen 5‑7) und klappe sie zunächst zusammen
            worksheet.Cells.GroupRows(4, 6, true);

            try
            {
                // Erweitere die gruppierten Zeilen mit ShowGroupDetail (isVertical: false für Zeilen, Index: 4)
                worksheet.Cells.ShowGroupDetail(false, 4);
                Console.WriteLine("ShowGroupDetail method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
            }

            // Speichere die Arbeitsmappe, um die Wirkung zu demonstrieren
            workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


