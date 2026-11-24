---
title: "SparklineGroupCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroupCollection-Methode. Fügt der Sammlung eine SparklineGroup mit einer Sparkline hinzu."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

Fügt der Sammlung ein [`SparklineGroup`](../../sparklinegroup/) mit einer [`Sparkline`](../../sparkline/) hinzu.

```csharp
public int Add(SparklineType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | SparklineType | Gibt den Typ der Sparkline-Gruppe an. |

### Rückgabewert

[`SparklineGroup`](../../sparklinegroup/) object index.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodAddWithSparklineTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Sparklines hinzufügen
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            try
            {
                // Rufen Sie die Sparkline-Gruppensammlung ab
                SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;

                // Rufen Sie die Add-Methode mit dem SparklineType-Parameter auf
                int index = sparklineGroups.Add(SparklineType.Line);

                // Konfigurieren Sie die Sparkline-Gruppe
                SparklineGroup group = sparklineGroups[index];
                group.Sparklines.Add("A1:A5", 5, 0);

                Console.WriteLine("Sparkline group added successfully with type: Line");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

Fügt der Sammlung ein [`SparklineGroup`](../../sparklinegroup/) mit einigen [`Sparkline`](../../sparkline/) hinzu.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | SparklineType | Gibt den Typ der Sparkline-Gruppe an. |
| dataRange | String | Gibt den Datenbereich der Sparkline-Gruppe an. |
| isVertical | Boolean | Gibt an, ob die Sparklines aus dem Datenbereich zeilenweise oder spaltenweise geplottet werden sollen. |
| locationRange | CellArea | Gibt an, wo die Sparklines platziert werden sollen. |

### Rückgabewert

[`SparklineGroup`](../../sparklinegroup/) object index.

### Hinweise

Diese Methode erstellt ebenfalls Sparklines. Wenn *isVertical* true ist, müssen die Anzahl der Zeilen in dataRange und locationRange gleich sein. Wenn *isVertical* false ist, müssen die Anzahl der Spalten in dataRange und locationRange gleich sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionMethodAddWithSparklineTypeStringBooleanCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten für Sparklines hinzufügen
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(3);
            sheet.Cells["C1"].PutValue(8);
            
            // Sparkline-Gruppe mit angegebenen Parametern hinzufügen
            sheet.SparklineGroups.Add(
                SparklineType.Line, 
                "A1:C1", 
                false, 
                CellArea.CreateCellArea("D1", "D1")
            );
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


