---
title: "Cells.GetRowOriginalHeightPoint"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die ursprüngliche Zeilenhöhe in Punkt angegeben zurück, wenn die Zeile ausgeblendet ist."
type: docs
url: /de/net/aspose.cells/cells/getroworiginalheightpoint/
---
## Cells.GetRowOriginalHeightPoint method

Gibt die ursprüngliche Zeilenhöhe in Punkt zurück, wenn die Zeile ausgeblendet ist.

```csharp
[Obsolete("Use Cells.GetRowHeight(int,bool,CellsUnitType) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetRowOriginalHeightPoint(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Cells.GetRowHeight(int,bool,CellsUnitType). Diese Methode wird 12 Monate nach April 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowOriginalHeightPointWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Speichere die ursprüngliche Höhe vor der Änderung.
            double originalHeightBefore = cells.GetRowOriginalHeightPoint(0);
            
            // Zeilenhöhe ändern.
            cells.SetRowHeight(0, 25.5);

            try
            {
                // Ursprüngliche Höhe nach der Änderung abrufen.
                double originalHeight = cells.GetRowOriginalHeightPoint(0);
                double currentHeight = cells.GetRowHeight(0);

                Console.WriteLine($"Original row height: {originalHeight} points");
                Console.WriteLine($"Current row height: {currentHeight} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowOriginalHeightPoint: {ex.Message}");
            }

            workbook.Save("GetRowOriginalHeightPointDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


