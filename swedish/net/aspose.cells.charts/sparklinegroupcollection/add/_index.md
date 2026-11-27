---
title: "SparklineGroupCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroupCollection‑metod. Lägger till en SparklineGroup med en Sparkline till samlingen"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

Lägger till en [`SparklineGroup`](../../sparklinegroup/) med en [`Sparkline`](../../sparkline/) till samlingen.

```csharp
public int Add(SparklineType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | SparklineType | Anger typen av Sparkline‑gruppen. |

### Returvärde

[`SparklineGroup`](../../sparklinegroup/) object index.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för sparkline-diagram
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            try
            {
                // Hämta Sparkline‑gruppsamlingen
                SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;

                // Anropa Add‑metoden med SparklineType‑parameter
                int index = sparklineGroups.Add(SparklineType.Line);

                // Konfigurera Sparkline‑gruppen
                SparklineGroup group = sparklineGroups[index];
                group.Sparklines.Add("A1:A5", 5, 0);

                Console.WriteLine("Sparkline group added successfully with type: Line");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

Lägger till en [`SparklineGroup`](../../sparklinegroup/) med några [`Sparkline`](../../sparkline/) till samlingen.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | SparklineType | Anger typen av Sparkline‑gruppen. |
| dataRange | String | Anger dataområdet för Sparkline‑gruppen. |
| ärVertikal | Boolean | Anger om sparklines ska plottas från dataområdet radvis eller kolumnvis. |
| locationRange | CellArea | Anger var sparklines ska placeras. |

### Returvärde

[`SparklineGroup`](../../sparklinegroup/) object index.

### Anmärkningar

Denna metod kommer också att skapa sparklines. Om *isVertical* är true måste antalet rader i dataRange och locationRange vara lika. Om *isVertical* är false måste antalet kolumner i dataRange och locationRange vara lika.

### Exempel

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
            
            // Lägg till exempeldata för sparkline-diagram
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(3);
            sheet.Cells["C1"].PutValue(8);
            
            // Lägg till Sparkline‑grupp med angivna parametrar
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

### Se även

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


